# Operational Limitations

To maximize the performance of Aurora, it's important to be mindful of its performance capabilities and how it responds when pushed to its limits. In addition, it's crucial to follow best practices for operating in challenging conditions.

## Flight Control

When operating in flight modes other than Manual, tilt angle and vertical speed are limited to 12 degrees and 0.7 m/s, respectively, when flying below an altitude of 2 meters. This measure aims to prevent tip-overs during landing, but it may decrease speed when flying below the takeoff point, such as when conducting surveys from a high location.&#x20;

## Continuous Flight

If you have extra batteries or a good charger, you can continually fly your Aurora; the limitation is the battery capacity.&#x20;



{% hint style="warning" %}
When the weather is hot, it's advisable to have 2 extra batteries on hand. This is because the batteries that were just used will need time to cool down before they can be charged to the appropriate temperature (50 degrees).°C).
{% endhint %}

## Environment&#x20;

Aurora can operate in temperatures between -20 and 50 degrees Celsius, making it suitable for both position mode and survey flying. However, it's crucial to be cautious when operating in extreme temperatures.



{% hint style="warning" %}
For the best performance, avoiding exposing the Herelink handset to direct sunlight is recommended. Although it can operate in temperatures up to 50C if kept in a shaded area and being charged, it's important to maintain peak performance during extreme weather conditions.&#x20;

One way to achieve this is to charge the Herelink while in use. Excessive heat or cold can significantly decrease the battery life and may lead to unexpected shutdowns.

&#x20;To prevent overheating, keeping the screen brightness below 50% is advisable.
{% endhint %}

## Wind

When operating the Aurora drone in windy weather conditions, it is essential to approach cautiously. As the altitude increases, the wind's strength also rises, making it risky to fly the drone if the wind speed exceeds 40mph. If the wind speed is a significant fraction of the drone's maximum speed, it can negatively affect control in all flight modes.&#x20;

Therefore, taking the necessary precautions to ensure a safe and successful flight is crucial. \
For optimal safety, installing propeller protectors and keeping them on when the drone is not being used is advisable. This will reduce the likelihood of hazardous propeller spin caused by strong winds. It is also recommended to avoid using drones in hazardous conditions to ensure secure flying.

{% hint style="danger" %}
If you need to fly the Aurora in high winds, you can modify the MPC\_XY\_VEL\_MAX values. However, please do not exceed 22m/s 50mph.
{% endhint %}

## Rain and Dust

Please note that while the Aurora drone is designed to be highly water-resistant, flying it in rainy conditions is not advisable. It's important to remember that most payloads are also not waterproof. Additionally, it's recommended to avoid dusty or sandy areas as the intake filter may not be able to capture all tiny dust particles, despite the drone's enclosure having openings for cooling.

## Radio Interference

When a signal becomes weak due to interference or long range, it can cause a disconnection with the aircraft, which triggers the failsafes. It is important to properly configure the failsafes to avoid this scenario, especially if you anticipate encountering a weak signal.

## Range

When using Herelink, it is important to remember that the range can extend up to 2 miles in optimal conditions if the patch antenna is directed towards Aurora and there is no interference. However, it is essential to be aware that radio interference from other sources, such as Wi-Fi networks, can decrease the range.&#x20;

It's important to note that obstructions such as buildings and trees, especially those in the direct line of sight between Herelink and Aurora, can greatly diminish the range.
