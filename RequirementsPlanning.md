# Requirements and Planning
This file contains all the components for section 1.1 of the task - Requirements and Planning \
As directed by the headings, this file will contain sections 'User Stories', 'Use Cases' and 'Requirements', in that order. 

## User Stories - Functioncal Requirements
This section will contain all 10 of the user stories for the assignment. \
The main actors referred to will be the scientists, engineers and various service workers. \
The secondary actors referred to will generally be the database, and sensors (a wide array of sensors for different devices).

### General Functional Requirements
1. 'Parking' the wind turbine in the event of a blizzard. 
2. Keeping track of where all the vehicles are - tracking software - in case a rescue is needed. 
3. Monitor the status of data collection systems (need for maintenance, have a regular test encoded, to run regularly, as scheduled tests). 
4. Monitor, and change the status of the living quarters - ensure suitable living conditions (temperature, air quality, etc.) - functionality to change temperature, 
5. Communicating with the outside world, in the case of emergencies. 
6. Keep track of weather cycles and to forewarn the inhabitants to any incoming weather disasters. 
7. Software to keep track of current food supplies and future incoming food supply (i.e. food status). 
8. Software to automatically, or manually, map the environment outside, and detect any major changes to the landscape. 
9. Monitor the electrical requirements and production of the entire base. This would include monitoring the fuel available for the generator, and alerting when a need arises, and the state of the battery, automatically performing regular tests. Collect requirement statistics periodically.
10. Know what season/time of year it currently is, to be able to make use of the solar panels when possible. 


### User Story 1 - Turbine Parking
As a service worker, I want to be able to 'park' (shut down operations and (somewhat) pack up) the wind turbine in the event of a blizzard, to avoid damage to the turbine. 

### User Story 2 - Vehicle Tracking
As staff on the base, I want to be able to track where all the vehicles for the base currently are, so that I can easily locate them to use in the event of an emergency. 

### User Stories 3.1 & 3.2 - Data Collection System Monitoring
As a service worker, I want to be able to monitor the current status of the data collection systems, to either know when scheduled maintenance is required, or be alerted if extra maintenance is required. \
As a scientist, I want to be alerted when/if a data collection systsem isn't working, to know to disregard data collected during a potentially faulty period.

### User Story 4 - Living Quarters Monitoring
As a scientist, I want to be able to monitor the livability conditions of the living quarters, so that I can ensure a safe living standard. 

### User Story 5 - Outside World Communication
As staff on the base, I want to be able to communicate with the outside world, so that I can contact people in the case of an emergency. 

### User Story 6 - Weather Tracking
As a scientist, I want to be able to view the upcoming weather patterns to be able to prepare the base for any incoming weather disasters. 

### User Story 7 - Monitoring Food Supplies
As staff on the base, I want to be able to see the current status for the available food on the base, as well as be alerted of any unforseen circumstances, to be able to develop a ration plan, and a plan to deal with the situation going forth as soon as possible. 

### User Stories 8.1 & 8.2 - Environment Mapping
As staff on base, I want to be alterted to any drastic changes to the external landscape outside, to be able to develop a plan to deal with any changes. \
As a service worker, I want to be able to manually map the external landscape to be able to verify any major and impactful environment changes. 

### User Stories 9.1 & 9.2 - Monitor Electrical Requirements and State
As an engineer, I want to be able to view the electricity requirement and production to be able to ensure stable supply and demand of electricity. \
As a service worker, I want to be able to be alerted when the battery needs maintenance/is non-functional, so that I can perform the maintenance or sort out a new battery.\
*Calculate and store base electrical requirements in the database periodically*

### User Stories 10.1 & 10.2 - Solar Panel Use
As an engineer, I want to be alerted when the solar panels are available to be effectively used, so that I can increase the electrical production for the base. \
As a service worker, I want to be alterted when the solar panels are available to be effectively used, so that I can run diagnostics on the power system, and get it ready for use. 

## Use Cases
This section contains all the use case stories; an extension on user stories 7, and 9. 

### Use Case 1 -
Goal: \
Primary actor: \
Secondary actor(s): \
Precondition: \
Trigger: \
Flow of events: \

Extensions: \

### Use Case 2 - 
Goal: \
Primary actor: \
Secondary actor(s): \
Precondition: \
Trigger: \
Flow of events: \
Extensions: \

### Use Case 3 - Monitoring Electrical Requirements and State
As an engineer, I want to be able to view the electricity requirement and production to be able to ensure stable supply and demand of electricity. \
Goal: Manage current status of overall electrical system\
Primary actor: Engineer\
Secondary actor(s): Database, sensors\
Precondition: Engineer is logged onto system (with valid engineer credentials)\
Trigger: Engineer selects option to view overall electrical system\
Flow of events: \
1. Sensors on the active production devices (solar panels (if summer), wind turbine, battery, generator) detect how much power is being produced, and send the information to the database.
2. Database retrieves most recent statistics for electrical consumption on the base.
3. System retrieves production and usage statistics from database.
4. System displays the production and usage statistics side by side, with a comparison metric for production to usage.
5. 
Extensions: \

### Use Case 4(?) -
Goal: \
Primary actor: \
Secondary actor(s): \
Precondition: \
Trigger: \
Flow of events: \

Extensions: \

## Use Case Diagram
The use case diagram is included in a separate file, entitled UseCaseDiagram. 

## Non-Functional Requirements
### Usability Requirements
Usability requirements are requirements that directly relate to how useable the software is, and showcase how the software increases efficiency. \
For example the easy location and use of the software features. 
#### Usability Requirement 1
The software must be able to access all features in a maximum of 3 clicks on the interface.

#### Usability Requirement 2


#### Usability Requirement 3


#### Usability Requirement 4
The software must have a system to validate inputs for certain functions, which need inputs to either be a specific type or within a certain range.

### Performance Requirements
Performance requirements are, logically, the requirements that relate to the softwares performance. \
This performance is commonly things like how efficiently the resources are used, how quickly it responds to an event and its' data processing speed. \
All the performance requirement tests should be performed on the computers that are available on the antarctic base. It should be noted that all the tests don't need to be performed explicitly on the base, but with the same hardware available on the base.
#### Performance Requirement 1
The system must be able to perform an action requested by a user within 15 seconds 99.99% of the time.

#### Performance Requirement 2
The system must be able to be able to process data at a rate of 30 megabits/second.

#### Performance Requirement 3
The system should be able to process the electricty production data from the sensors (accessed through the database) 

### Reliability Requirements 
Reliability requirements are requirements of the systems reliability. \
These requirements acknowledge an imperfect world, and imperfect software standards, but set some standards of what the software **must** be able to do. 
#### Reliability Requirement 1
The systems communication functionality must be available to use 99.99% of the time, as in an emergency, it is a vital function. \
The systems vehicle tracking functionality must also be available 99.99% of the time, as it is a very important feature in a crisis.

#### Reliability Requirement 2
The system is expected to fail on only 0.1% of attempts when a user tries to make use of any incorporated function.\
A failure would be described as just an error message, rather than the entire system crashing.

#### Reliability Requrement 3
The mean time between failure for the weather tracking functionality should be 4 months.\
This is an important feature due to the significant effect a unexpected weather anomaly can have on the base (e.g. blizzard causing the turbine to be parked. If the turbine isn't parked, damage can occur to the device).
