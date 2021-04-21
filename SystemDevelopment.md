# System Development 
This file will include all the information covering the assignment section 1.2 - System Development 

## 1.2.1 Work Breakdown Structure (wbs)
This section will include the complete work breakdown structure. This will include the task name, time taken (in ) to complete the task, and dependancies. \

* 1.0 Setting up the Base
    * 1.1 Implement a link between all each of the sensors and actuators with the system, to be used in whatever way is required.
    * 1.2 Develop a GUI for user interaction

* 2.0 Establish Communication Systems Software
    * 2.1 Implement software to link the communications devices with the system.
    * 2.2 Implement software to send communications to the outside world, using the communication systens.

* 3.0 Set Up Software for Weather Sensing
    * 3.1 Establish a software link between the sensors to detect current weather and the system.
    * 3.2 Use communication systems in the software to get weather
 information for upcoming weather cycles
    * 3.3 Use local weather prediction tools for shorter term weather conditions (that is used and checked more often)
    * 3.4 Software to automatically send (with a manual override option) base-wide alerts for a soon upcoming weather anomaly (such as a blizzard).

* 4.0 Develop Software to Monitor Electrical Systems
    * 4.1 Implement software to turn off/on the solar panel production system based on light (using sensors, and predicted upcoming light based on weather). Should include an alert to service worker users when its ready.
    * 4.2 Periodically measuring production from production systems, then uploading the data to the database
    * 4.3 Measure usage from data collection devices, and overall base operations.
    * 4.4 Develop software to retrieve data from the database for both and display it in a comparison table for viewing by engineers.
    * 4.5 In the case where there is a lower than expected energy production, an option is to be programmed to allow engineers to alert service workers

* 5.0 Develop Software to Monitor Food Supplies
    * 5.1 Recieve user input when food is taken from supplies - updates database.
    * 5.2 Implement features to alert the staff when stocks get low.
    * 5.3 Software to use communication systems to order more food when the food stocks are low.

* 6.0 Turbine Parking
    * 6.1 Program the software to periodically use upcoming and current weather information to determine if the conditions are suitible for the turbine to run, alerting the service workers if they are not.
    * 6.2 Use software in conjunction with actuators to allow service workers to be able to park the wind turbine.

* 7.0 Living Quarters Monitoring
    * Implement software to periodically use sensors to measure the air quality in the living quarters, as well as the average base temperature (indoors). The software should altert the scientists in a case when either metric is out of a preset range.
    * The software (accessible by scientists or engineers) should have options to change the range for either metric, to account for electrical supply, or any situational changes.

* 8.0 Monitor Status of Data Collection Systems
    * 8.1 Program the software to use actuators and sensors to periodically perform simple diagnostic tests to verify the systems are working as expected. If any systems are not working, the software should note the last date the system was working, then alert scientist and service worker accounts.
    * 8.2 The software should alert service worker accounts regularly for scheduled maintenance of the collection systems.

* 9.0 Post Blizzard Checks
    * 9.1 An automated (with a manual option) mapping feature to be implemented in the system to use cameras to map the external landscape of the base after a major weather anomaly (such a blizzard), to detect any largescale changes to the base. Service worker accounts should be alerted of these changes
    * 9.2 Implement software to automatically perform simple diagnostic tests on data collection systems, as well as electrical production systems to verify the functionality of each. In the case either is not working, all staff accounts should be alerted.

* 10.0 Vehicle Tracking 
    * 10.1 All the staff should be able to access the feature in the system that uses software tracking to show the location of all the bases vehicles on a map.

* 11.0 Testing
    * All the testing of the software should be done on hardware that has the same capabilities as the computers on the antarctic base. 1/3 of the requirements and software testing should be done in Australia, with the other 2/3 being conducted on the base, with the preexising system still in use.

Task | Estimated Duration (days) | Dependancies | ES | EF | LS | LF | ST |
:----|:-------------------------:|:-------------|:--:|:--:|:--:|:--:|:--:|
**Start** | - | - | - | - | - | - | - |
**1.1** |13|none | 0 | | | | |
**1.2** |20|1.1 | 0 | | | | |
**2.1** |5|1.2 | | | | | |
**2.2** |5|2.1 | | | | | |
**3.1** |2|1.2 | | | | | |
**3.2** |2|2.2, 3.1 | | | | | |
**3.3** |2|1.2 | | | | | |
**3.4** |3|3.2, 3.3 | | | | | |
**4.1** |3|3.2, 3.3 | | | | | |
**4.2** |3|4.1 | | | | | |
**4.3** |2|1.2 | | | | | |
**4.4** |2|4.2, 4.3 | | | | | |
**4.5** |1|4.4 | | | | | |
**5.1** |1|1.2 | | | | | |
**5.2** |2|1.2 | | | | | |
**5.3** |1|5.1 | | | | | |
**5.4** |3|5.3, 2.2 | | | | | |
**6.1** |3|3.2, 3.3 | | | | | |
**6.2** |3|6.1 | | | | | |
**7.1** |2|1.2 | | | | | |
**7.2** |2|7.1 | | | | | |
**8.1** |5|1.2 | | | | | |
**8.2** |1|1.2 | | | | | |
**9.1** |8|1.2 | | | | | |
**9.2** |5|1.2 | | | | | |
**10.1** |5|1.2 | | | | | |
**11.0** |40|all (final block)| | | | | |
**Finish** | - | - | - | - | - | - | - |

## 1.2.2 AON Graph

## 1.2.3 Critical Path
Based on the AON graph, the critical path would be as follows:
