# JHS-HVAC-Assignment
Digital Electronics (non-PLTW) Course

In this project, you will use your knowledge of flowchart programming with fischertechnik ROBOPro (available to download [here](https://www.fischertechnik.de/en/service/downloads/robotics)) to create a single-room HVAC system. Passing the project means completing all design deliverables set by the customer below.

[//]: # (Image References)

[image1]: https://github.com/joshrwhite/JHS-HVAC-Assignment/blob/master/Images/Rubric_PhysicalDesign.PNG "Rubric1"
[image2]: https://github.com/joshrwhite/JHS-HVAC-Assignment/blob/master/Images/Rubric_SoftwareDesign.PNG "Rubric2"


## Design Brief

A hospital is currently in the planning stages of their new pediatrics ward. They've asked your automation team to develop the central air system for their NICU (newborn intensive care unit). Newly born infants require steady high heats to continue growing healthily. Your team must design and present a model of a system that controls temperature based on user settings identified by best practices. Using an NTC resistor as the analog input and a lamp and fan (or series of lamps and fans) as outputs, model a system which will supply a constant temperature to a single room. It is expected that the fan or lamp will be running variably depending on the input temperature resistance but they are not required to run at full capacity to maintain steady tempurature. In other words, if little heat is required, only little heat will need to be given. (Efficient HVAC systems usually don't have heaters and blowers running at full capacity.) The program must be able to track how long the lamp and fan run as well as any time that neither is running in order to calculate wattage and, in turn, cost. Since the infants will be in a controlled environment, your team should have a control panel indicating whether the fan or lamp is running.

## Further Project Requirements

1. The design and prototype implementation must be completed using fischertechnik components and the ROBOPro programming software.
2. Comments in the code should communicate each function's intended purpose clearly.
3. The final write up is professional with descriptive pictures of the physical prototype and HVAC program.
4. A final video is provided (which can easily be linked through the use of a markdown (.md) file).
   - The [writeup_template.md](https://github.com/joshrwhite/JHS-HVAC-Assignment/blob/master/writeup_template.md) file in the repository, can be used to fulfill requirements 3 & 4.
5. The final submission will be a link to your GitHub repository for this project, so please maintain a professional digital environment.
6. While successful completion of the project means that the design constraints found in the Design Brief are met, A+ work will be awarded to projects that show creativity in meeting these objectives.

## Rubric

Physical Construction:

![Rubric1][image1]

ROBOPro Programming Software:

![Rubric2][image2]

## Repository Navigation

Aside from the `README.md` file and supporting documents, there is an `.rpp` file for examples of HVAC functions that meet most, but not all of the design constraints. The example ROBOPro program shows the basic branch and variable functions needed for a closed-loop system. These can be mimicked, but blatant plagiarism will be penalized.

There is also a `writeup_template.md` file which can be used as a starting point for the final report.

## Downloading ROBOPro

After going to the download [URL](https://www.fischertechnik.de/en/service/downloads/robotics), click on the "ROBOPro" down arrow. Install using the "Update ROBOPro 4.4.4 (MSI, 266MB)" version as the Demoversion will not allow compatibility with a ROBO Interface or TX/TXT Controller. Make sure to install all drivers so that the USB is able to be read by the computer.
