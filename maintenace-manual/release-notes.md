# Release Notes

## AOS 3.3.9

#### What's new <a href="#what-improved.1" id="what-improved.1"></a>

* Allow manufacturers to override the Skynode default Wifi access point SSID using the AP\_CONFIGURE\_AP\_SSID environment variable.
* New radio statistics are included in the Ulog file uploaded to the suite. This will simplify radio troubleshooting
* Disable AuterionOS serial console on production images

#### What improved <a href="#what-improved" id="what-improved"></a>

**Payloads**

* Do not force the video streaming frame rate to a fixed value. This can reduce video latency by 30-50ms.
* Fix the issue where the video was getting recorded correctly on the Sony A7R camera, but AMC reported that the recording failed

**Sony A7R/ILX**

* Enable exposure control settings also in video mode
* New picture profile setting exposed to AMC
* Read all settings ranges from the camera to avoid trying to change settings that are not available for a specific camera model or in a specific camera state
* New movie recording settings exposed to AMC
* Remove "flash" white balance setting
* Do not allow user to change to manual focus if the lens does not support it
* Limit shutter speed range to 1/4000
* Decouple exposure mode, exposure compensation, ISO, shutter speed, aperture, and focus mode settings depending on whether the camera is in photo or video mode.
* Fix SD card status and error reporting.
* Fix the the movie format setting. Previously, users could set values that were temporarily unavailable due to other setting combinations.
* Set AuterionOS date and time to camera during initial connection
* Read focus level from the camera to improve the manual focus support
* New Sony 50mm and Samyang 75mm lens support
* Fix the issue that would cause the Sony camera to stop working if plugged out and back into Skynode via USB
* Fix an issue that would cause the Sony camera capture feedback not to work when switching between USB flash drive and camera SD card storage.

**Radios**

* Improve doodle labs radio support. This will allow pairing with doodle labs radios to be faster and more reliable.

**Others**

* Fix an issue that could happen during photo upload to the suite. This could cause all other suite features to malfunction.
* Fix issue that could cause the AuterionOS web UI to not get updated or to get corrupted when updating from a release with the old web UI
* Fix issue that could cause the FMU hardfault log upload to the suite to fail during AuterionOS bootup
* Improve error messages in AuterionOS update API to report API version incompatibilities
* Fix app remove button and make sure that also app settings are removed. The action could fail randomly.
* Improve error handling during AuterionOS app installations
* Fix issue where AuterionOS could get stuck at boot if a USB flash drive was plugged in during power up
* Fix issue where last digits of the Auterion suite API key were visible in some AuterionOS REST API responses
* Fix issue that caused excessive memory usage by the modem driver in AuterionOS when when modem was not in a configurable state
* Disable app actions in the AuterionOS web UI while the drone is armed
* During skynode soft reboots the USB hub could stop working. Now AuterionOS makes sure the USB hub is alive during every boot up.
* Fix issue where the app update status was not successful although the app installation had succeeded
* Fix issue with modem metrics that could cause the CPU to spike every time AuterionOS requested the metrics from the modem.
* Various optimizations are related to the connection to the suite. The service also used a lot of resources when the vehicle was not connected to the Internet.

## AMC 1.30.17

### **What's new** <a href="#whats-new" id="whats-new"></a>

* Pilot Profile: after logging in with the Suite account AMC will provide the following pilot information:
  * Display the pilot name, icon, and email.
  * Display Operator ID in AMC.
  * Display the list of pilot certificates available in the suite and the expiration date for each of them.
  * Add support for opening certificates as PDFs.
* Mission Manager:
  * A New Mission Actions bar with the following actions was added in Plan View: Mission menu, Save, Clear, and Upload.
  * Add the ability to import missions to AMC.
  * Add the ability to filter missions.
  * Efficiency and stability improvements.
* Gimbal information:
  * Add the gimbal model, vendor, and firmware version in the About section.
  * Notify the user if the gimbal needs a firmware update.
* Connection Manager:
  * Improved support for Doodle Labs radio.
  * Improved the process of connecting to the vehicle:
    * New UI/UX design.
    * Created an improved step-by-step guide.
* Non-modal pop-ups: battery info and GPS pop-ups can be left open while the user interacts with AMC and will not auto-close when the user clicks outside the pop-up.
* New VTOL Straight landing pattern: end a mission by descent to the transition point in a straight line.
* Cursor on Target changes to comply with program Acheron requirements.
* Add the ability to assign external flight modes to joystick buttons.
* Added coordinate units to first time user setup.

### **What's improved** <a href="#whats-improved" id="whats-improved"></a>

* General performance improvements: RC controller messaging, camera projection, compass indicator, camera mode change, camera settings, task monitor.
* FreeFly Pilot Pro joystick improvements:
  * Fix the joystick dead band setting and add a default value of 4%.
  * Map joystick R1 button to camera trigger action.
* Mission improvements:
  * Survey mission: fix upload of preset settings.
  * Extras tab: unified UI design.
  * Mission estimator: reset total flight time to 0 when deleting all the mission items.
  * Fix mission upload progress bar size.
  * Fix importing KML mission files on Android versions greater than 10.
  * Custom mission items: add custom mission actions in AMC non-Advanced-Mode.
* Fix the Autotune procedure that is stuck in the process.
* Start the ATAK video stream without any manual settings needed.
* Fix the Go To action: use the altitude value of the previous action as default.
* Fix System Health; the status is not always updated.
* Left tools strip action labels are now visible by default.
* Fix home position does not update when only altitude changes.
* Fix the first-time user setup that is missing the skip button.
