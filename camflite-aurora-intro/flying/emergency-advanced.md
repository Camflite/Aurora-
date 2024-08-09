# Emergency/Advanced

## General Guidance

Aviation safety should always prioritize human safety above everything else. While an aircraft can be replaced, human lives are invaluable. In any emergency, it is vital to prioritize the safety of oneself and others over preserving the equipment or the aircraft. Emergencies are unpredictable and may not fit into pre-defined categories, but having a comprehensive understanding of aircraft systems, piloting proficiency, and sound judgment can significantly increase the chances of achieving the best possible outcome. Proper maintenance, using checklists for normal procedures, and carefully planning pre-flight can substantially reduce the chances of emergencies. The pilot's diligence is crucial in ensuring a safe flight before takeoff and during operation. In most emergencies, three basic actions can be taken.

* Maintain aircraft control
* Analyze the situation
* Take appropriate action.

{% hint style="warning" %}
If the drone behaves abnormally, do not continue to fly land immediately. Contact Camflite for further instructions.  Any anomaly should not be ignored; it is better to be safe than sorry.
{% endhint %}

During an emergency, the pilot needs to keep visual contact with the aircraft to prevent small issues from becoming bigger problems. Once the situation is under control, it is necessary to identify the cause of the emergency and take the appropriate action. In most cases, this involves landing the aircraft as soon as possible, as it can always be replaced.

### Return Mode

During emergencies, it's important to not solely rely on Return Mode as it may not be effective due to potential aircraft performance issues or loss of GPS signal. It's advisable to have alternative contingency plans and strategies to ensure a safe outcome in an emergency.

{% hint style="danger" %}
<mark style="color:red;">When landing or maintaining aircraft control becomes impossible, the Emergency Stop should only be considered a last resort.</mark>&#x20;
{% endhint %}



When considering the need to perform an emergency stop on an aircraft, it is essential to remember that doing so while the aircraft is in the air would result in a catastrophic crash. Therefore, if an emergency stop is necessary, it must be executed in a location as far from people as possible to minimize the risk of harm or damage to others. Exploring all other options and prioritizing safety before resorting to an emergency stop is crucial.



## Error and Warning Indication&#x20;

The aircraft uses Auterion Mission Control (AMC) status indicators on the pilot handset or PC to communicate the presence of errors and warnings. Most messages are accompanied by an audible message, such as "Return Flight Mode". Moreover, the Aurora boom LEDs will start flashing when the battery level is low.

Status messages, including errors and warnings, are stored in Flight Logs. After an emergency, review the log to determine the source of the problem.

If the meaning of an error or warning is unclear, don't hesitate to contact Camflite Support. Share as many details as possible, including the flight log.

## Emergency Procedure Checklists

The Aurora checklists provide concise instructions to mitigate risks resulting from hardware, connection, or pilot errors. Further details are provided below.

### Loss of Orientation

If the aircraft's orientation is lost, neutralizing the inputs and activating the position mode are recommended. The next step is to work on identifying the front of the aircraft. We suggest using a "guess and check" method consisting of small roll-right inputs while yawing the aircraft 90 degrees at a time. Using a roll input rather than pitch is better because lateral motion is easier to see at a distance than fore/aft motion.\
\
If it is impossible to identify the orientation and it is safe to activate the Return Mode, we recommend doing so. In Return Mode, by default, the aircraft will yaw to put the front towards the direction of flight after climbing.

Resume flying or land as necessary.

### Unexpected Aircraft Behavior

If the Aurora aircraft behaves erratically, perform the following steps: neutralize inputs, activate Position Mode, and observe the aircraft. If it continues to fly in an uncommanded manner in Position or Altitude Mode, switch to Manual Mode.

In some cases, unexpected behavior may occur due to degraded GPS signals or erroneous sensor readings. Return Mode may not behave reliably in such cases. However, Manual Mode does not rely on these sensors.

Land as soon as possible.



{% hint style="warning" %}
If the drone does anything out of the norm, contact Camflite for help.
{% endhint %}

### Landing Detector Failure

If the aircraft bounces back into the air or remains on the ground with the propellers still spinning after touching down, it's possible that the autopilot did not register the landing. In this case, you should climb up and try landing again with a greater downward speed.

{% hint style="info" %}
Landing the aircraft firmly will give the accelerometers and gyroscopes a sufficient contrast between flight and landing.
{% endhint %}

If an attempted landing in Position and Altitude mode is unsuccessful, land in Manual Mode.&#x20;

If an attempted landing in Manual Mode is unsuccessful, perform an Emergency Stop with the aircraft on the ground or as close as possible.

### Loss of GPS

If the GPS connection is lost during flight, the aircraft will switch to (Altitude Mode), and GPS-reliant flight modes such as Position, Return, and Mission will not be available.

{% hint style="info" %}
It is the pilot's responsibility to be proficient with altitude and manual mode and to have the aircraft configured safely in case of GPS loss.
{% endhint %}

Examples of behavior without GPS:

* If GPS is unavailable when arming the device, the Home Point will not be set, and Return Mode will be unavailable during the flight. Even if GPS becomes available later, Return Mode will not be available.
* If the pilot tries to enter Return Mode, an error will be displayed on the pilot's handset, and the aircraft will remain in its current mode (Altitude or Manual).
* If Land Mode is activated, for example, due to a failsafe, the aircraft will descend as if it were in Altitude mode. It will maintain a consistent attitude but drift with the wind. However, it's worth noting that the pilot cannot activate Land Mode because it requires GPS.
* If GPS is lost during a mission, the aircraft will display a warning and switch flight mode to either Altitude Mode or Manual Mode, depending on the degradation of the signal.&#x20;
* Loss of GPS due to electronic connection issues can lead to total loss of control.
* If GPS provides altitude information, such as when using (RTK GPS), the Altitude Mode's ability to maintain altitude accurately may be affected if GPS is lost.

### RC Loss of Signal (LOS)

RC Loss of Signal (LOS) can occur if the pilot's handset signal degrades or stops or Aurora doesn't receive the signal due to distance or interference (e.g., obstacles or other radio signals).

A failsafe mechanism will be activated if the remote control signal is lost longer than the RC Timeout. The RC Timeout is set to 0.5 seconds, which may not allow enough time for the pilot to react before the failsafe mechanism is triggered. By default, the failsafe mechanism will activate the Return Mode.

If the signal is lost, check the power and orientation of the pilot's handset antenna, especially when Aurora is far from the pilot.

If the signal is recovered, the pilot can take control by moving the sticks or pressing a flight mode button.

{% hint style="info" %}
Please note that there are two types of signal losses in RC (remote control) systems: Loss of Signal (LOS) and Data Link Loss. LOS refers to the SBUS data stream containing the pilot's inputs, while Data Link Loss refers to the stream of MavLINK messages. Aurora routes both data streams through a single radio system. It is important to remember that during operation, the AMC (Aurora Mission Control) app must be in the foreground on the pilot handset. Otherwise, the Data Link will fail after 30 seconds and trigger a failsafe. So, if the AMC app is closed or running in the background, the Data Link will fail, and the failsafe will be triggered.
{% endhint %}



### Loss of Video Signal

Video signal loss can occur if the aircraft flies out of range or behind an object that blocks the signal. The best way to regain control of the aircraft is to maintain visual contact. This can be achieved by the pilot seeing the aircraft or using a visual observer.

Yawing the aircraft can improve signal reception if the aircraft body is blocking the line of sight between transmitter and receiver antennas.

If the video signal or visual contact is lost, activate Return Mode to bring the aircraft back within signal reception range.

{% hint style="danger" %}
As a pilot, it is your responsibility to be vigilant and avoid any potential collisions with other aircraft or obstacles. During flight, you must maintain a direct line of sight with Aurora and adhere to the see-and-avoid requirements mandated by local regulations. Additionally, you may use visual observers as needed to ensure the safety of your operations.
{% endhint %}

## Failsafes

AMC configures failsafe behavior and settings. The AMC documentation covers each failsafe and related setting in detail.

Some failsafes are discussed briefly below.

{% hint style="warning" %}
We highly recommend using the default settings and only modifying the Return Altitude unless you're an expert user who has extensively tested the impact of changes.
{% endhint %}

### Low Battery

Battery level is evaluated based on the State of Charge (SoC, e.g., 72%), not voltage (e.g., 23 Volts).

The aircraft safely lands when the battery level of the aircraft becomes low, and the autopilot system can take action. However, the system's default settings do not intervene until the battery level becomes very low. Furthermore, the low battery failsafes cannot determine the position or distance of the aircraft from its Home Point. Therefore, the pilots are responsible for monitoring the battery level and ensuring the aircraft safely lands on the ground.

| State     | SoC (default) | Action (default)       |
| --------- | ------------- | ---------------------- |
| Warning   | 20%           | Warning: Audio Message |
| Critical  | 15%           | Return Mode            |
| Emergency | 6%            | Land Mode              |
