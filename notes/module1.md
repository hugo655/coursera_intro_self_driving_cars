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

## Notes on Lesson #3
Imagine the scenario where a driver stops at an interception. Several decisions may be taken 
depending on how the intersection is configured. Example:
* Is there a pedestrian-crossing? if so, the car has to stop behind it. If there isn't? where
should the car be stopped?
* Are there any cars behind?
* Are there any cars in the intersection when the red light turns green?

Driving requires a lot of immediate decisions!

One approach to model this would be by using **Rule Based Planning**. In which a series of rules
dictates the next behaviour: 
* Example: If there is a stop sign. Stop

An alternative approach would be **Predictive Planning**, which predictions are made based on
how objects are moving on the field of the car. 
* Example: A car has stopped for 10 seconds, hence is is likely that is going to remain stop for a couple 
of more seconds.

This second type of planning is more aligned to how humans think, and thus how most self-driving 
vehicles work in the present.

[This Paper](https://ieeexplore.ieee.org/abstract/document/7490340) is a good survey
on motion planning for self-driving vehicles.

[This other paper](https://onlinelibrary.wiley.com/doi/epdf/10.1002/rob.20255) diccusses some
of the challenges of motion planning in urban area. It used 'mixed planning systems'.
