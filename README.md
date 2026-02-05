<!--
Hey, thanks for using the awesome-readme-template template.  
If you have any enhancements, then fork this project and create a pull request 
or just open an issue with the label "enhancement".

Don't forget to give this project a star for additional support ;)
Maybe you can mention me or this repo in the acknowledgements too
-->
<div align="center">


![Logo](assets/Hardware_Image_1.png)

# Electric Eel-Inspired Battery For Implantable Medical Devices 

This project is an AI-powered automatic medication dispenser designed to improve medication adherence using a combination of image recognition, OCR, and natural language processing. The system is built for patients, caregivers, and healthcare providers to ensure safe and timely medication intake — all while being monitored remotely through a mobile app.

It integrates hardware control (Arduino), YOLO-based pill recognition, and a custom-trained spaCy NLP model to extract dosage and frequency instructions from prescription labels. A PyQt6 desktop interface manages the system on-device, and a mobile app enables remote supervision. 

All the resources I used for this project can be found in the following Google Drive, linked for your reference: https://drive.google.com/drive/folders/1BSqckdxfqDh0ZibXCd9fYPzXVN9h-TSW 


**This project is not currently licensed for use or redistribution. All rights reserved.**


[![Contributors](https://img.shields.io/github/contributors/SophieBarriault/Electric-Eel-Inspired-Battery-For-Implantable-Medical-Devices)](https://github.com/SophieBarriault/Electric-Eel-Inspired-Battery-For-Implantable-Medical-Devices/graphs/contributors)
[![Last Commit](https://img.shields.io/github/last-commit/SophieBarriault/Electric-Eel-Inspired-Battery-For-Implantable-Medical-Devices)](https://github.com/SophieBarriault/Electric-Eel-Inspired-Battery-For-Implantable-Medical-Devices)
[![Forks](https://img.shields.io/github/forks/SophieBarriault/Electric-Eel-Inspired-Battery-For-Implantable-Medical-Devices)](https://github.com/SophieBarriault/Electric-Eel-Inspired-Battery-For-Implantable-Medical-Devices/network/members)
[![Stars](https://img.shields.io/github/stars/SophieBarriault/Electric-Eel-Inspired-Battery-For-Implantable-Medical-Devices)](https://github.com/SophieBarriault/Electric-Eel-Inspired-Battery-For-Implantable-Medical-Devices/stargazers)
[![Issues](https://img.shields.io/github/issues/SophieBarriault/Electric-Eel-Inspired-Battery-For-Implantable-Medical-Devices)](https://github.com/SophieBarriault/Electric-Eel-Inspired-Battery-For-Implantable-Medical-Devices/issues)
[![License](https://img.shields.io/github/license/SophieBarriault/Electric-Eel-Inspired-Battery-For-Implantable-Medical-Devices.svg)](https://github.com/SophieBarriault/Electric-Eel-Inspired-Battery-For-Implantable-Medical-Devices/blob/main/LICENSE)

[View Demo](https://drive.google.com/file/d/1wByr87FT2HsipwZgwH-gzBg_70QS4TUb/view?usp=sharing) ·
[Documentation](https://github.com/SophieBarriault/Dispenser/blob/main/README.MD)  ·
[Report Bug](https://github.com/SophieBarriault/Dispenser/issues) ·
[Request Feature](https://github.com/SophieBarriault/Dispenser/issues)

 
</div>

---

# 📔 Table of Contents

- [Abstract](#-Abstract)
  - [Demo Video](#-screenshots)
  - [Materials Used](#-Materials-Used) 
- [Introduction](#-Introduction)
  - [Current Work](#-Current-Work) 
  - [Solution](#-Solution)
- [Methods ](#-Methodst) 
  - [Protocol](#-Protocol) 
- [Contact](#-contact)
- [Acknowledgements](#-acknowledgements-) 


---

## 🌟 Abstract

	Many implantable medical device users rely heavily on said devices, from things like insulin pumps to pacemakers, meaning that they should spend as little time as possible without their device’s usage. However, because many of these devices are electrically powered, many a time the battery of these devices has to be replaced, which in some cases can result in risky surgeries. While these surgeries don’t have to be performed often, only every couple of years, being without these life-saving devices can still pose risks to patients’ health. In order to solve this issue, this project aims towards the development of an electric eel-inspired battery designed as a better alternative for implantable medical devices batteries, in order to eliminate the need for periods where users are without their devices. In order to do so, the battery will be built with various cells of stacked hydrogel plates, that mimic the electricity-generating specialized cells found in electric eels called electrocytes, and will use an ion gradient found within the artificial electrocyte, hydrogel stacks in order to generate electricity, similarly to how electric eels do. 
***Keywords: Chemistry, electrochemistry, engineering, biomedical engineering, physics, medical apparatus, medicine, biology***





### 📷 Demo Video 

Click to watch the demo here! 

[![Watch the Demo Video](assets/to_demo.png)](https://drive.google.com/file/d/1wByr87FT2HsipwZgwH-gzBg_70QS4TUb/view?usp=sharing) 


---

### 👾 Materials Used 

- **Python** – Core programming language for the application

- **Toga** – GUI framework for building cross-platform desktop and mobile apps 
- **Buildozer** - GUI framework for both Android and IOS compatibility 

- **OpenCV** – Real-time image processing and integration with camera for pill verification

- **Tesseract OCR** – Optical Character Recognition for extracting text from prescriptions

- **spaCy** – Custom Named Entity Recognition (NER) model to extract dosage/frequency info

- **YOLOv8** – Object detection model to monitor pill intake and hand movement

- **Flask** – Lightweight server to handle requests between the app and ML models

- **PySerial** – Communication between the Python app and the Arduino board

- **Arduino** – Controls pill dispensing mechanism (via servo motors, etc.)

- **Git & GitHub** – Version control and project collaboration

---

### 🎯 Features

- **Automated Pill Dispensing** 
  Dispenses the correct medication at the right time using an Arduino-controlled mechanism, reducing the risk of missed or incorrect doses.

- **Real-Time Pill Intake Monitoring** 
  Utilizes a YOLOv5-based image recognition system to track the sequence: pill present → pill taken → hand empty — confirming successful medication intake.

- **Custom OCR Processing** 
  Uses Tesseract OCR to extract medication names, dosages, and instructions from images of prescriptions or labels.

- **Medical NER Model** 
  A custom-trained spaCy Named Entity Recognition (NER) model processes OCR output to identify key medical information like dosage frequency and medication schedules.

- **Cross-Platform Interface (Toga + Buildozer)** 
  Built using the Toga framework for both desktop and mobile (Android and IOS) platforms, allowing caregivers and users to interact with the system easily.

- **Flask-Based Communication** 
  A lightweight Flask server connects the app to backend ML models, ensuring fast and reliable processing of user input and image recognition results.

- **Emergency Alert System** 
  If a user fails to take their medication within a set time frame, the system plays an audio alert and notifies a connected caregiver.

- **Time-Based Triggers** 
  The application runs on a schedule, automatically activating the camera and dispenser based on predefined medication times.

- **PDF Report Generation** 
  Extracted text from prescriptions is automatically saved and compiled into a downloadable PDF for easy recordkeeping and sharing with healthcare providers.


--- 


<!-- Getting Started -->
## 	:toolbox: Introduction 

Tens of millions of people in the world rely on implantable medical devices in their day-to-day lives, with an estimated 25 million people in the U.S. relying on them alone ((Singh et al., 2021). Despite this international heavy reliance, implantable medical devices often have one big flaw: their batteries’ longevity. The longevity of a devices’ battery relies on a multitude of factors, including device type and usage, which in turn affects the replacement cycle and overall cost of the medical devices (Challenges of Batteries for Implantable Medical Devices: Miniaturization and Biocompatibility, 2025). When implantable devices require replacement, depending on what kind of device they are, in some cases they require surgery, like pacemakers. While the surgeries aren’t always necessarily at the highest risk, surgeries in general can carry risks like complications and long recovery times, especially when they’re performed close to organs, like the heart, for things like pacemakers, which isn’t optimal for patients. Additionally, being without the implantable medical device that a patient relies on for their day-to-day life due to needing to recharge/replace the battery isn’t optimal either, as it leaves the patient vulnerable, even if it’s just for a moment. For example, when an insulin pump user has to recharge their insulin pump battery, in that period, they can be at risk of hyperglycemia and diabetic ketoacidosis if not monitored properly. Because of the issues and risks that come with traditional implantable medical device batteries, an alternative solution is needed that’ll mitigate the need to replace and/or charge said batteries. 


<!-- Prerequisites -->
### :bangbang: Current Work 

The only work about electric eel-inspired batteries specifically was published in 2017 by researchers at the University of California, San Diego in a paper titled An electric-eel-inspired soft power source from stacked hydrogels. My approach in this paper is based on the approach from the paper from 2017, however concentrations and materials used are altered in order to best fit my project’s goals, as the paper from 2017’s goal was just to be able to test whether or not the hydrogel stacks could generate electricity. While the original paper’s approach was successful in generating some voltage, the researchers were only able to generate around 1 to 2 volts of electricity, which is not enough for what my project aims to do, which is power implantable medical devices. Currently, the other alternatives that exist to this issue are energy storage devices, such as rechargeable lithium batteries, human body energy harvesters, through kinetic energy harvesting, and wireless power transfer, through things such as radiofrequency radiation. However, all of these current solutions are either invasive, which can be dangerous to patients, contain harmful materials that are not biocompatible with the human body, or do not generate enough electricity and do not have high longevity. 

<!-- Run Locally -->
### :running: Solution 

My project focuses on creating a type of battery that’s able to produce its own electricity using an ion gradient in order to generate electricity, similarly to how an electric eel does so. By creating such, patients won’t have to be without the devices they rely on for periods of time due to replacement and/or charging. There is a need for this solution in order to reduce the amount of surgeries and risks associated with normal battery replacements in implantable medical devices, and the medical complications that come with them/that they can lead to. Unlike current alternatives to traditional implantable medical device batteries, like energy storage devices, human body energy harvesters, and wireless power transfer, my solution aims to not be invasive, does not contain any harmful materials, generates enough electricity to power medical devices, and is able to last for a long time. 

<!-- Deployment -->
### :triangular_flag_on_post: Methods 

The location is my house and the Billerica Memorial High School. The materials used are CMC (Carboxymethyl Cellulose), NaPA (sodium polyacrylate), Chitosan, NaCl (deionized kosher salt), glycerol, alginate powder, and water, that will be deionized. All materials will be obtained from Amazon and the equipment available at my school. The equipment used are a scale, 250 mL beakers, pipettes, non-contact thermometer, acrylic plates (petri dishes), a whisk, a hot plate, a ruler, a multimeter, graphite electrodes, and proper personal protective equipment (PPE), specifically lab goggles and gloves. I am planning on working with a local advice mentor that was provided to me by the Massachusetts Science and Engineering Fair (MSEF) as well as my advisors from my school’s Science National Honor Society chap

<!-- FAQ -->
## :grey_question: Protocol: 

**Anionic Gel:**
1. Heat 100 mL deionized water to 50 - 60 °C. 
2. Add 0.5 g agar and stir until fully dissolved.
3. Add 1.0573 g NaPA, stir gently until thickened. 
4. Pour into an acrylic, such as a petri dish, into an even 1 mm layer and let rest until solid. 
5. Cut out 12 1 mm thick circles, with a radius of 1 mm. 
**High Concentration Gel:** 
6. Heat 100 mL deionized water to 50 - 60 °C. 
7. Slowly sprinkle 2 g CMC while stirring vigorously until fully dissolved (make sure to break up any clumps). 
8. Add 0.5 g agar and stir until fully dissolved.
9. Add 3 g (2.922 g) NaCl and dissolve. 
10. Pour into an acrylic, such as a petri dish, into an even 3 mm layer and let rest until solid. 
11. Cut out 24 1 mm thick circles, with a radius of 1 mm. 
**Low Concentration Gel:**  
12. Heat 100 mL deionized water to 50 - 60 °C. 
13. Slowly sprinkle 2 g CMC while stirring vigorously until fully dissolved (make sure to break up any clump). 
14. Add 0.5 g agar and stir until fully dissolved.
15. Add 0.0877 g NaCl and dissolve. 
16. Pour into an acrylic, such as a petri dish, into an even 3 mm layer and let rest until solid. 
17. Cut out 12 1 mm thick circles, with a radius of 1 mm. 
**Cationic Gel:** 
18. Combine 22.22 mL of 4.5% acetic acid to 77.78 mL of deionized water to make 100 mL of 1% acetic acid solution. (This allows for our chitosan to solution ratio to be around 1:1, which is a general rule of thumb for dissolving chitosan). 
19. Slowly add 0.787 g chitosan powder while stirring overnight, or stir vigorously with a blender on high speed, at a temperature of 50 - 60 °C until the chitosan is completely dissolved and no particles can be seen. 
20. Add 0.5 g agar and stir until fully dissolved. 
21. Pour into an acrylic, such as a petri dish, into an even 1 mm layer and let rest until solid.
22. Cut out 12 1 mm thick circles, with a radius of 1 mm. 
**Stack:** 
23. Stack the layers in repeating order, from top to bottom: 
High Concentration → Anionic → Low Concentration →  Cationic → High Concentration 
24. Stack 12 of these stacks on top of one another. 
25. Place graphite electrodes flat against the outer faces of the stack.
26. Connect wires of a multimeter to electrodes outside the gel, with the positive wire touching the top electrode, nearest to the first anionic gel, and the negative wire touching the bottom electrode, nearest to the last cationic gel. 



 
<!-- Contact -->
## :handshake: Contact

Sophie Barriault - [Linkedin](www.linkedin.com/in/sophie-barriault) - sophiebarriaultofficial@gmail.com 

Project Link: [https://github.com/SophieBarriault/Dispenser/tree/main](https://github.com/SophieBarriault/Dispenser/tree/main)


<!-- Acknowledgments -->
## :gem: Acknowledgements 

Useful resources and libraries that I've used in my project: 


 - Link to all technical sources used: https://drive.google.com/drive/folders/1BSqckdxfqDh0ZibXCd9fYPzXVN9h-TSW?usp=drive_link 
 - [Shields.io](https://shields.io/)
 - [Awesome README](https://github.com/matiassingers/awesome-readme)
 - [Emoji Cheat Sheet](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#travel--places)
 - [Readme Template](https://github.com/othneildrew/Best-README-Template) 






































