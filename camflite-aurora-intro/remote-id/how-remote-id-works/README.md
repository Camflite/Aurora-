# How Remote ID works

## Broadcast Method

The current Remote ID implementation in AuterionOS on Skynode is using the WiFi Beacon transmission method, where Remote ID information is embedded into [WiFi Beacon frames](https://en.wikipedia.org/wiki/Beacon\_frame). Every device that scans for WiFi networks and is within range therefore has access to the drone's Remote ID information.

## Remote ID Data

AuterionOS streams the basic ID message, aircraft location and system message from the GCS in every WiFi Beacon frame. More specifically, the frames contain:

* GCS Information:
  * Latitude and Longitude of the GCS
  * Geometric altitude of the GCS
* Vehicle information:
  * Vehicle serial number or session ID
  * Latitude and Longitude of the vehicle
  * Geometric altitude of the vehicle
  * Velocity of the vehicle expressed as
    * Track direction
    * Horizontal and vertical speed
* Coordinated Universal Time (UTC) timestamp of this data
* Operational or emergency status of the vehicle
