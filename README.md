# drone_interface
A framework for interfacing a drone controller with python.

## **Goal**
The initial goal of this project is to control a drone using Python. More specifically, a drone(such as the Eachine QX65) can be controlled with Python by interfacing a drone controller(such as the BetaFPV TX02) with a Raspberry Pi using digital potentiometers(such as the MCP42X1). *A secondary goal of this project is to develop an opportunity for exploring computer science and electronics.*

## **Key Ideas**
* By connecting to the drone controller/ radio with digital potentiometers - we can ignore brand specific protocols and allow for many types of drone radios to be used. *(Imagine that the digital potentiometers just take the place of the analog potentiometers that make up the radio gimbals.)*
* Having a ground station computer(Raspberry Pi, Desktop, etc.) control the drone radio can allow for more resource intensive flying and also allows for the groundstation computer to perform other tasks and link to other services. 

### **Current Limitations**
Without feedback from the drone - it is essentially flying blind. Two possible solutions to this:
1. Attach one or more time of flight(ToF) sensors to provide some basic telemetry.
    1. This data needs to then be sent back to the radio and then connected to the ground station computer. 
2. Utilize the drone OSD and scrape data using CV to control flight.
   
   2. This requires more work and is heavily dependent on the quality of the video feed.
  

