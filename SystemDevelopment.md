# System Development 
This file will include all the information covering the assignment section 1.2 - System Development 

## 1.2.1 Work Breakdown Structure (wbs)
This section will include the complete work breakdown structure. This will include the task name, time taken (in ) to complete the task, and dependancies. \

* 1.0 Setting up the Base
    * 1.1 Implement a link between all each of the sensors and actuators with the system, to be used in whatever way is required.
    * 1.2 Develop a GUI for user interaction - this includes user in 

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
    * 4.5 In the cae where there is a lower than expected energy production, an option is to be programmed to allow engineers to alert service workers

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
**Start** |- | - | - | - | - | - | - |
**1.1** |5|none |0|5|0|5|0|
**1.2** |8|1.1 |5|13|5|13|0|
**2.1** |5|1.2 |13|18|13|18|0|
**2.2** |5|2.1 |18|23|18|23|0|
**3.1** |2|1.2 |13|15|21|23|8|
**3.2** |2|2.2, 3.1 |23|25|23|25|0|
**3.3** |2|1.2 |13|15|23|25|10|
**3.4** |3|3.2, 3.3 |25|28|31|34|6|
**4.1** |3|3.2, 3.3 |25|28|25|28|0|
**4.2** |3|4.1 |28|31|28|31|0|
**4.3** |2|1.2 |13|15|29|31|16|
**4.4** |2|4.2, 4.3 |31|33|31|33|0|
**4.5** |1|4.4 |33|34|33|34|0|
**5.1** |1|1.2 |13|14|29|30|16|
**5.2** |2|1.2 |13|15|28|30|15|
**5.3** |1|5.1, 5.2 |15|16|30|31|15|
**5.4** |3|5.3, 2.2 |23|26|31|34|8|
**6.1** |3|3.2, 3.3 |15|18|28|31|13|
**6.2** |3|6.1 |18|21|31|34|13|
**7.1** |2|1.2 |13|15|30|32|17|
**7.2** |2|7.1 |15|17|32|34|17|
**8.1** |5|1.2 |13|18|28|33|15|
**8.2** |1|8.1 |18|19|33|34|15|
**9.1** |8|1.2 |13|21|26|34|13|
**9.2** |5|1.2 |13|18|29|34|16|
**10.1** |5|1.2 |13|18|29|34|16|
**11.0** |40|all (final functional block)|34|74|34|74|0|
**Finish** |- | - | - | - | - | - | - |

## 1.2.2 AON Graph
The AoN graph is included in the repository under the name AoN_Graph.png
## 1.2.3 Critical Path
The Critical Path is the path that has no slack time, i.e. if any of these tasks is held up, the entire duration of the project increases.\
All the tasks on the critical path have a slack time of 0. \
Based on the AON graph, the critical path would be as follows:\
1.1 -> 1.2 -> 2.1 -> 2.2 -> 3.2 -> 4.1 -> 4.2 -> 4.4 -> 4.5 -> 11.0 \
The critical path is also indicated on the graph, with the line being red, rather than black.

