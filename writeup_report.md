# JHS-HVAC-Assignment

[//]: # (Image References)

[image1]: https://github.com/HunterDProfessional/My-Hvac-Assignment-/blob/master/image/bill.jpg "bill"
[image2]: https://github.com/joshrwhite/JHS-HVAC-Assignment/blob/master/Images/Rubric_SoftwareDesign.PNG "Rubric2"

## Design Criteria  
•	Using fischertechniks and ROBOPro, build a prototype HVAC system to maintain a certain tolerance of temperature 
•	A light should indicate whether the fan or the lamp is on 
•	A control panel should count the number of seconds the fan or lamp has been on • Fully comment all functions within the flowchart program 

Design  
Physical  
To complete the cooling, we mounted a fan with two propellers (four blades) directly over the temperature sensor. This was wired to the M1 output on the circuit board.  
To complete the heating, there were three lights wired in parallel around the heat sensor. They were wired to the M2 output.  
There were lights wired to the motor and lights in parallel (one for motor, one for lights). These were the indicator lights.  
 
 
 
 
Code  
A kill switch was coded in, but it has no effect on the rest of the code.  
![bill][image1] 
 
We created the code so that the program would check if the temperature was between predetermined values. Depending on what they were it would heat or cool at low, medium, and max power.  
![image1][image2] 
 
The extreme ends had no limit. The ranges for heating were at high, medium and low, respectively, were <350, >350 and <370, >370 and <390. The ranges for cooling for high, medium, and low, respectively, were >450, <450 and >430, <430 and >410. The ideal temperature was set to 400, with an acceptable range of +/- 10.  
 
 
The cut off for the extreme ranges was easy. They were simply when the resistor passed a determined value. The other four settings also required a system that would cut it if they surpassed the value, but they additionally needed to be refreshed regularly in case the system was heating up or cooling down faster than that setting could cool or heat it.  
![image2][image3] 
 
The AX is the sensor override, while the A is the timer. A wait of only 0.1 second was used to make sure that the temperature override was checked regularly.  
 
Next, a system was used to turn off the motor(M1) and lights(M2) and reset the time counter to 
0. This then fed back into the start of the program where it checks and acts upon the temperature.  
![image3][image4] 
 
 
 
 
Here is an overall picture of the code:  
![image4][image5] 
 
It is annotated for better explanation (I was told to).  
