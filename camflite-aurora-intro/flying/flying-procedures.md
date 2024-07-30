# Flying Procedures

## Aurora Check List

Below is a PDF you should print and keep to check before every flight.&#x20;

{% file src="../../.gitbook/assets/Aurora Check list.pdf" %}

## Issues Preventing Arming

You may occasionally encounter issues that will prevent Aurora from arming; please follow the next steps to resolve any issues-

## Compass Calibration

If AMC asks you to calibrate the compass and won't allow you to take off, follow the instructions to recalibrate sensors in an area without significant magnetic interference (far from large metal structures or magnetic/electric installations).&#x20;

## Everything else&#x20;

Check if the AMC message you're encountering is on our Error/Warning Spreadsheet, and follow the associated instructions. If you're still experiencing the issue, don't hesitate to contact support@camflite.com for further troubleshooting.&#x20;

## Arming and Disarming

Aurora's propulsion system has two fundamental states: Disarmed and Armed.

| State    | Definition                                  | Indication |
| -------- | ------------------------------------------- | ---------- |
| Disarmed | Safe mode, no spinning propellers           | None       |
| Armed    | Aircraft will spin propellers, ready to fly | None       |

Aurora can be armed with or without GPS.&#x20;

{% hint style="info" %}
Pro Tip: Wait for GPS lock even if you don't plan to use Position Mode because Return Mode relies on GPS.
{% endhint %}

{% hint style="danger" %}
Before arming, ensure people and other obstacles are clear of the propellers. Be prepared for Aurora to take off.
{% endhint %}

The manual transitioning between armed and disarmed states is via the pilot handset throttle stick. (The pilot's handset default configuration is [Mode 2](https://docs.px4.io/master/en/getting\_started/rc\_transmitter\_receiver.html#types-of-remote-controls).)

| State           | Input                                                                                 |
| --------------- | ------------------------------------------------------------------------------------- |
| Arming (Mode 2) | Hold the throttle stick down and right for 2 seconds.                                 |
| Disarming       | When the aircraft has landed, continue holding the throttle stick down for 2 seconds. |

{% hint style="info" %}
It is not possible to disarm via the normal method while in flight.

To disarm during flight, perform an Emergency Stop.
{% endhint %}

{% hint style="info" %}
If Aurora does not arm, check Auterion Mission Control (AMC) for errors or warnings.
{% endhint %}

{% hint style="info" %}
Only use the throttle stick to Arm & Disarm. Aurora will not respond to two-stick input (i.e. DJI arming gesture). However, you can use the takeoff icon to arm and take of your Aurora automatically.
{% endhint %}

Missions may Arm and Disarm the aircraft automatically. For example, if a mission is started while the aircraft is disarmed on the ground, the aircraft will arm and take off.

### Automatic Disarm Methods

Under these conditions, Aurora will automatically disarm.

| Method                                                                              | Aurora behavior                                                                                                                                        |
| ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Gon the round timeout before taking off                                             | If Aurora sits on the ground at idle throttle for 10 seconds, it will automatically disarm.                                                            |
| Land mode                                                                           | If Aurora is in Land Mode and detects a landing, it will disarm after 1 seconds. For example, this applies if the last command in a mission is "Land." |

### Automatic Disarm Methods



Under these conditions, Aurora will automatically disarm.

| Method                                                                       | Aurora behavior                                                                                                                                       |
| ---------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| Ground timeout before taking off                                             | If Aurora sits on the ground at idle throttle for 10 seconds, it will automatically disarm.                                                           |
| Land mode                                                                    | If Aurora is in Land Mode and detects a landing, it will disarm after 1 second. For example, this applies if the last command in a mission is "Land". |

## Taking off



Position Mode is best for taking off in most cases, as it offers the most stabilization. However, taking off in Altitude, Manual, and Mission modes is certainly possible.&#x20;

For 5 seconds after takeoff, the maximum pitch and roll angles are reduced to 12 degrees.

After takeoff, promptly climb out of the ground effect (i.e., to 3 feet / 12 meters of altitude) to avoid snagging landing gear on the ground.

{% tabs %}
{% tab title="Position and Altatude " %}
Once you have armed the aircraft, ensure that the throttle stick is returned to its central position. At this point, the propellers will be spinning. To initiate takeoff, simply raise the throttle stick. As a result,  the aircraft will lift off the ground.
{% endtab %}

{% tab title="Manual Mode" %}
To prepare for takeoff, first arm the device. Then, hold the throttle stick straight down while avoiding any Yaw input. When ready, slowly raise the throttle stick. The propellers will start to accelerate as soon as the throttle stick moves. Once the throttle reaches the mid-point, there will be sufficient thrust to take off. Keep raising the throttle to achieve a smooth and brisk takeoff.
{% endtab %}
{% endtabs %}

## Landing

Position Mode is best for landing in most cases, as it offers the most stabilization. However, it is also possible to land in Altitude and Manual modes. The aircraft behaves a little differently in each mode.



{% hint style="danger" %}
Do not hand-catch Aurora. The aircraft is designed to be landed on hard flat surfaces away from people. Hand-catching can result in serious injury or death.
{% endhint %}

In Position and Altitude Modes, at altitudes below 6 feet, the maximum vertical speed is reduced to 0.7 m/s (from the normal value of 2 m/s).

Aurora will disarm automatically after the autopilot detects a landing. Landing detection brings input from several sensors to determine when it is safe to disarm.

{% hint style="warning" %}
If the landing is undetected (i.e., the props do not stop after touchdown), perform the Emergency Procedure for Landing Detector Failure.
{% endhint %}

{% tabs %}
{% tab title="Landing in Postion" %}
In order to successfully land your aircraft, you should first raise it to a height of at least 2 meters. Then, gradually decrease throttle input by pulling the throttle stick directly downward without making any pitch, roll, or yaw adjustments. The landing sensor on Aurora will manage the descent speed automatically. Once the aircraft reaches the ground, keep the throttle stick down until Auroa disarms and the propellers stop completely.\
\
It's important to keep in mind that if you're operating at altitudes below 2 meters, the maximum pitch and roll angle is limited to 12 degrees. This limitation is in place to prevent any sudden maneuvers that could cause the aircraft to tip over.
{% endtab %}

{% tab title="Landing in Altitude " %}
When switching to Altitude Mode during landing, it's important to remember that the pilot is responsible for controlling the lateral velocity of the aircraft. Although the autopilot regulates the descent rate by managing the throttle, the pilot must actively monitor and control the lateral speed.\
To initiate the landing process, hover the aircraft at a height of 2 meters above the intended landing area using minimal pitch and roll commands to reduce lateral speed and pitch/roll angles. Then, push the throttle stick downwards to begin the descent.\
After touchdown, keep the throttle stick in the downward position until the Aurora disarms and the propellers come to a complete stop. This will ensure a safe and controlled landing.\
It's important to note that when operating at altitudes below 2 meters, there are limitations on the allowable pitch/roll angles. These limits are reduced to 12 degrees to minimize the risk of sudden movements that could cause the aircraft to tip over.
{% endtab %}

{% tab title="landing in manual" %}
When switching to Manual Mode for landing, the pilot takes on more responsibility for controlling the aircraft's vertical and lateral velocity. To begin the landing process, hover the aircraft above the desired landing spot at a height of at least 2 meters. Use gentle pitch and roll commands to maintain a slow lateral speed and minimize pitch/roll angles.&#x20;

Gradually reduce the throttle to allow the aircraft to descend smoothly. As the aircraft approaches the ground and enters the ground effect, the pilot may need to lower the throttle even further to maintain a controlled descent.&#x20;

Once the aircraft touches down, quickly reduce the throttle to zero to prevent bouncing or dragging of the landing gear. It's important to keep the throttle stick down until the aircraft disarms and the propellers completely stop spinning, ensuring a safe landing.
{% endtab %}
{% endtabs %}

## Battery Changes / Hotswaps

{% hint style="danger" %}
The Aurora aircraft has a failsafe feature that automatically directs it back to the launch point when the battery level is low. Unfortunately, this mechanism cannot detect obstructions or potential problems that might hinder a safe landing before the battery is entirely depleted. If the failsafe is triggered while the aircraft is far from the launch point, there may not be enough battery power to complete the return journey. Hence, it falls to the pilot to assess the situation and decide when to replace the battery to ensure a secure landing.
{% endhint %}

