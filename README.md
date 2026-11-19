Industrial Conveyor Sorting System | PLC Project 2

About This Project

I developed this project to improve my practical understanding of PLC programming and industrial automation.

The idea was to simulate a conveyor system that can detect products, control a sorting mechanism and respond to stop or overload conditions.

I built the control logic using OpenPLC Editor and Ladder Diagram (LD) programming. This helped me understand how different sensors, motor commands and internal memory bits work together in an automated system.

Software Used

* OpenPLC Editor
* Ladder Diagram (LD)
* macOS

How the System Works

The system uses a conveyor motor to move products through a simulated sorting process.

When the required operating conditions are satisfied, the conveyor motor can run. The program uses sensor signals and internal memory to determine when the sorting pusher should activate.

I also included stop and overload protection logic. These conditions can prevent the motor from running and require the appropriate recovery steps before restarting.

Main Features

* Conveyor motor start and stop control
* Product detection and rejection logic
* Automatic sorting pusher control
* SET and RESET memory functions
* Stop and overload interlocks
* Restart protection and reset logic

Ladder Logic Development

I organised the PLC program into 12 labelled rungs.

The rungs cover conveyor motor operation, sorting pusher control, reject memory, sorting memory and restart protection.

Working with these different functions helped me understand how ladder logic can be divided into smaller sections to make a control system easier to follow and troubleshoot.

Testing and Results

I tested the program using the OpenPLC debugging environment.

During testing, I confirmed that:

* The conveyor motor switched ON when the required start and operating conditions were satisfied.
* The motor switched OFF when the start signal was removed.
* The sorting pusher activated when the required motor, reject memory and sorting position conditions were met.
* The sorting pusher deactivated when the sorting position signal was removed.
* A stop condition disabled the conveyor motor and activated stop restart protection.
* An overload condition stopped the motor and activated the restart-required flag.
* The overload restart-required flag cleared when the reset input was activated.
* After overload recovery and reset, the conveyor could restart when commanded.

These tests helped me understand the importance of checking both normal operation and fault conditions in PLC programs.

What I Learned

This project gave me more confidence in reading, developing and testing ladder logic.

I gained practical experience with PLC inputs and outputs, sensor-based control, internal memory bits, SET/RESET instructions, safety interlocks and debugging.

I also learned how important it is to test different operating conditions rather than assuming a program will work correctly.

Project Screenshots

The screenshots folder contains five images covering all 12 ladder-logic rungs.

Project Scope

This project was developed and tested using software simulation in OpenPLC Editor.

It does not use a physical conveyor, industrial PLC or connected sensors and actuators. My aim was to build a stronger foundation in industrial control logic before progressing to hardware-based automation projects.