In the second-year of the Electrical and Electronics Engineering programme at The Hague University of Applied Sciences we were faced 
with the challenge of designing a bike-computer for a well known producer in home-training appliances. The requirements for this project were: 
1. If start is pressed, the lcd of the hometrainer will start counting upwards, displaying the time that the user was busy biking 
2. If recovery (after start) is pressed the hometrainer will hold the time the user were biking until the motor has reached its initial (0) state
3. If pause (after start) is pressed the hometrainer will hold the time, but if start is pressed afterwards the motor will start and the hometrainer will proceed counting from where it was stopped
4. The RPM must be calculated then shown on the LCD-display for 3 seconds and after 3 seconds the RPM must be updated
5. A motor-controller must be designed. The hometrainer is driven by an h-bridge so the motor position can be controlled by writing digital output to the h-bridge 
6. The hall-sensor and buttons on the hometrainer are not debounced, so therefore a debouncer is necessary. The total time that all switches bounced were 100 us. 
7. An estimation of the distance-biked must be shown on the display 

This project was finished successfully and acts as proof that each individual who had worked on the project-design are capable of designing complex-digital systems with minimal guidance from an external party or individual. 
For this project i was responsible for designing and testing of the datapath and control for the LCD-timer so the timer-output could be controlled and accurately displayed. Furthermore, I had also designed a debouncer and a module 
to calculate and update the rpm, however these are not included in the final design but are to be found in my github repository. This was not a requirement but out of interest i had also designed a mountain-climb-mode module
which causes the resistance of the wheel to increase after 1 minute until the maximum level has been reached. 

--13-04-2022: Updated my  project with 1. A fully working testbench displaying all input, internal and output signals
--						   2. Managed to reduce amount of logic cells without any reduction in performance by doing some adjustments in the module components