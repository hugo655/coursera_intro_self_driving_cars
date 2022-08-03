# Notes on Lesson #1

Driving task may be decomposed into minor subtasks:
* Perceiving;
* Planning the route;
* Controlling the device;

The concept of [Operational Design Domain](https://www.autonomousvehicleinternational.com/news/connectivity/autonomous-vehicle-safety-standard-defines-operational-design-domain-for-avs.html)
may also be applied to the scope of self-driving vehicles. This term has to do
with IT-LAW legal issues. 

The are some standards that deals with **classification of the automation level**, 
**Society of Automotive Engineers** deals with defining how much automatized is a 
given vehicle by answering questions such as:
* Does the driver needs to interact the steering wheel?
* Can the vehicle cross lanes?

Driving task can be broken into separated control systems:
* Lateral Control - Action of moving left and right on a given path
* Longitudinal Control - Action like break and accelerate
* Object and Event Detection and Response (OEDR) - Detecting things and reacting to disturbances
* Planning - Long planning (what roads to take) short planning (when to cross lanes)
* Miscellaneous - Signaling, buzzing ...

Level 0 - No automation

Level 1 - Either longitudinal Control or Lateral control (not both)
* Adaptive Cruise Control: Driver still needs to steer
* Lane Keeping Assistance: Driver still controls the speed

Level 2 - Partial Driving Automation : Both Laretal and and Longitudinal Control
* GM Super Cruise and Nissan ProPilot Assist

Level 3 - Conditional Drivinf Automation: Logitudinal, Lateral Control and ODER - The
driver does not need to interact but still needs driver alertness for emergencies

Level 4 - High Driving Automation no need of driver, but limited to certain conditions 
no need of driver alertness

Level 5 - High Driving Automation with no physical restrictions like the weather


# Notes on Lesson #2
How perception works? What are the goals? 

Any driving task requires OEDR (object and event detection and response). To Perceive the sytem
must **identify** and **understand it motions**. As humans, we can do such task easily, but for
machines is not so trivial. 

**Static Objects** are road marks, traffic lights, Road signs ... things that don't change.
**Dynamic objects** are either 2 wheelers (bikes and motocycles), 4 wheelers and pedestrians.

**Ego localization** are metric that can make the system identify its own position, velocity,
orientation. 

Some of the non-trivial challenges to perception are misreads from the sensors. Particularly:
* Reflection;
* Lens-flair (illumination directly into the sensor);
* Visibility for weather conditions;
