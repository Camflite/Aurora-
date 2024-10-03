# Pro Tips



### Camera Settings

AMC provides control of these settings in flight by pressing the ![](../.gitbook/assets/image.png) icon on the right of the screen while in Photo Mode:





<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

AMC will override these camera body settings:

* Shooting Mode dial, if set to P.
* Exposure Compensation dial, if set to 0.

Other camera body controls and menu options will be honored. For example:

* Focus Mode (e.g. wide, zone).
* Exposure Metering Mode (e.g. spot).
* Exposure Compensation dial, if set to non-0 value.

File type: JPG and RAW are available.



{% hint style="info" %}
We recommend selecting File Storage: Camera (SD card) when shooting RAW files. The system will store RAW files to USB, but the transfer time is prohibitively long, imposing a delay of several seconds between shutter releases.
{% endhint %}



### **Efficiency Tips**

Choose a survey flight path angle that minimizes the number of turns, essentially maximizing long, straight flight paths. For example, if you're surveying a complex next to a road that runs at a 30-degree angle, aligning the survey lines with the road may reduce the amount of maneuvering needed, resulting in shorter missions and better pictures.



Please remember the following information: \
\
To optimize efficiency and safety, rotate the survey entry and exit points to start and end at logical locations. It's best to begin at the furthest point from your takeoff location, as your mission will likely end closer to the home point when battery levels are most critical.\
\
Adjust the overlap and side-lap settings to suit your processing software and output type. AMC's default settings (70%) are a good starting point, but reducing these values can enable faster flight and greater area coverage. Lowering front overlaps will allow for faster flight during a mission, but ensure that the value is compatible with the processing software being used.

**Known issue:** Photos are not equally spaced in the flight direction, causing some minor variation in spacing. This may require a slightly larger forward overlap setting to ensure there is adequate overlap in every case.







Aurora can cover areas larger than 200 acres in a single flight at 2cm GSD. Here are some tips for flying these types of missions:

* When planning a mission, uncheck the "refly at 90°" option at the bottom of the Survey settings. This will cause Astro to fly only over the ground in single-direction passes instead of a cross-hatch pattern.
* If possible, fly from the center of a large survey to minimize the distance between the Herelink and Astro. The maximum telemetry distance is displayed in AMC during mission planning when you're at the takeoff location. Maintaining a line of sight to the vehicle throughout the survey is crucial for safety and ensuring a strong data link.
* Fly at 10-12m/s. The aircraft can fly up to 15m/s, but the flight time will actually increase if it is above 12m/s, resulting in a longer flight.
* A "typical" large area survey might have the following parameters: 12m/s speed, 120m altitude, 70% front overlap, 65% side overlap, and the gimbal angle pointing down (90°).
* Aurora defaults to limiting the distance between waypoints to 900 meters. This is a safety measure to prevent accidental waypoints from sending the drone out of range to unintended locations. However, in some rare cases, this may restrict the length of a survey. The distance between waypoints can be increased by adjusting the MIS\_DIST\_WPS parameter. It's important not to set this value larger than needed to maintain safety.
