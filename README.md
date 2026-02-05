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





### 📷 Example of Results 


[![Resullts from one trial stack](assets/to_demo.png)] 


--- 

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

<!-- FAQ -->
## :grey_question: Goals 

	In terms of milestones, the main milestones of my project will occur when the different types of hydrogels are successfully able to be formed and polymerized, when the hydrogel stacks are successfully able to generate volts of electricity, and when the hydrogel stacks are successfully able to generate 2 to 3 volts of electricity, and power an implantable medical device. The completion criteria for my project is defined as follows: the project must be able to generate its own electricity using the created ion gradient, must not rely on any external power sources for electricity, must be able to generate 3 volts of electricity as a maximum, and the final product must be biocompatible. I will test my project by measuring the voltage output using a multimeter, and I’ll evaluate my project based on the voltage output generated. In terms of performance specifications, bottom line, the battery must be able to output a consistent voltage without interruption of at least 2 to 3 volts. 

<!-- FAQ -->
## :grey_question: Risks  

	One of the main risks posed in this project is the usage and testing with electricity. However, the project does not exceed 120 volts and at most will generate 5 volts. Because of this, there’s no risk of arc flash events or internal component failure due to excessive voltage. Additionally, the power supply created also will not be serving more than one experiment at a time, reducing the risk of hazards created by switching between experiments. However, there’s still the risk of shock hazards, but none that can lead to serious physical harm. In order to minimize these risks, all experimentations related to electricity will be conducted in a lab environment, at school, that is supervised by adults. Additionally, proper personal protective equipment (PPE) will be worn at all times, including voltage-rated gloves and goggles. The Electrically Safe Work Condition (ESWC), according to the university of Virginia, will be applied as well as needed, ensuring that the battery never has any components that are removed in a hazardous way that could create a dangerous interruption in current. 

<!-- FAQ -->
## :grey_question: Results and Discussion (So Far)   

**Project Performance** 
		All the criteria set was successfully met and achieved in my project. With a single hydrogel stack, a stack was able to generate anywhere from 0.25 V to 0.31 V. In the calculated total voltage, given there’s no resistance, the total battery, with 12 stacks connected in series, should generate an output from 3 V to 3.72 V, which exceeds the criteria set. However, the resistance from the hydrogels themselves must be taken into account as well. 

**Challenges and Future Improvements** 
Despite its success, there’s some challenges I’d like to solve: 
- The gels need to be made sturdier, most likely via increasing the alginate concentration, as the alginate is what mostly gives the gels their structure. However, it also needs to be kept in mind to not add too much alginate to the point where the NaCl ion movements are inhibited.
- Thinner graphite electrodes are needed in order to ensure that the battery can be used for long periods of time without the gel stacks being crushed. The current electrodes being used work, but overtime might impede on the battery’s function.

There are also a few future improvements I’d like to work on as well: 
- The stacks need to be tested in various numbers in series in order to find the maximum voltage output.
- The battery needs to be tested with an implantable medical device. 
- The battery needs to be tested for long periods of time to ensure continuous voltage output.

<!-- FAQ -->
## :grey_question: Conclusion 

		These results demonstrate the viability of deploying a battery that’s able to generate and output its own voltage without the need for an external electricity source, showing how it can be used to help solve the issues of replacing and recharging the batteries in implantable medical devices. In conclusion, by addressing common faults in current solutions, such as the need for surgeries and leaving patients vulnerable for long times through recharging periods, this solution has the potential to prevent future side effects, enhance patient health, and introduce a biocompatible solution for this issue. 


<!-- FAQ -->
## :grey_question: References  

**References** 

Battery Components | Batteries | CAPLINQ. (2023). Caplinq. 
https://www.caplinq.com/renewable-energy/batteries/battery-components/ 

Blogionik. (2017, September 27). Blogionik. 
https://blogionik.org/blog/2017/09/27/biomimetic-potential-electric-eels/ Ahmed, E. M. 
(2013). 

Challenges of Batteries for Implantable Medical Devices: Miniaturization and Biocompatibility. 
(2025, September 3). Large-Battery.com. 
https://www.large-battery.com/blog/batteries-for-implantable-medical-devices-miniaturiz
ation-biocompat/ 

Electric eels inspired the first battery two centuries ago and now point a way to future battery 
technologies. https://doi.org/10.64628/aai.f7qrfpgac 

Hydrogel: Preparation, characterization, and applications: A review. Journal of Advanced 
Research, 6(2), 105–121. https://doi.org/10.1016/j.jare.2013.07.006 Jorgensen, T. (2022). 

Safety for Research | Environmental Health & Safety (EHS). (2024). Virginia.edu. 
https://ehs.virginia.edu/Electrical-Safety/Research Biomimetic potential of electric eels - 

Schroeder, T. B. H., Guha, A., Lamoureux, A., VanRenterghem, G., Sept, D., Shtein, M., Yang, 
J., & Mayer, M. (2017). An electric-eel-inspired soft power source from stacked 
hydrogels. Nature, 552(7684), 214–218. https://doi.org/10.1038/nature24670 Electrical 

Singh, P., Singh, G., & Kaur, G. (2021). Integrating Artificial Intelligence/Internet of Things 
Technologies to Support Medical Devices and Systems. Elsevier EBooks, 331–349.
https://doi.org/10.1016/b978-0-12-818576-6.00017-4 

Szymańska, E., & Winnicka, K. (2015). Stability of Chitosan—A Challenge for Pharmaceutical and Biomedical Applications. Marine Drugs, 13(4), 1819–1846. https://doi.org/10.3390/md13041819
‌




 
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






































