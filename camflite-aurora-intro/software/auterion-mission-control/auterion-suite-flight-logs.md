# Auterion Suite/Flight Logs

<figure><img src="../../../.gitbook/assets/Mouse Highlight Overlay 2022-05-18 10.19.13.png" alt=""><figcaption></figcaption></figure>

Manage your enterprise robotics program with Auterion Suite. The Suite is where your fleet data is collected, analyzed, and presented. Get insights on vehicles, assets, and operations to keep control over your robotics program. With Auterion-powered vehicles, data is delivered automatically and in real-time from the fleet to the Suite – while the drones are flying and without any manual intervention. [Learn more about the Auterion Suite here on Auterion's website.](https://auterion.com/enterprise/suite/)&#x20;



Aurora is built to integrate easily into the Auterion Suite, and many of Aurora's features are enabled through this platform.

* Manage your aircraft fleet.
* Access detailed flight logs, check vehicle status.
* Direct Camflite customer support with integrated flight log sharing and review
* Get software updates
* Aurora's live video-sharing capabilities&#x20;
* [Auterion's documentation](https://docs.auterion.com/suite) covers the Suite in depth.

## How to sign up for the Auterion Suite and Register your Aurora



* Using a computer, connect a USB-C cable from your computer to the IO panel on the underside of the Camflite Aurora.&#x20;
  * Power on the Aurora with batteries
  * **This physical connection to the Aurora is required for security reasons as the Suite enables location data, live streaming, etc.**
* Using a web browser, go to the following address to connect to the Aurora: **`http://10.41.1.1`**
* This page will allow users to sign up for the suite and automatically register and claim the aircraft. Click "Register Now" or scan the QR code to sign up on your mobile device.
  * Note: This requires the vehicle to be online to generate a signup QR code; otherwise, it’ll say “Internet required” for the registration prompt.
  * Connect the Aurora to the internet using these instructions to connect to either a WIFI or LTE network.&#x20;
  * If Aurora is connected to the internet and plugged into the computer and http://10.41.1.1 does not show the Register Now button, try refreshing your browser. &#x20;
* After completion, check for the Aurora unit under the "Vehicles" section on the Auterion Suite main dashboard.
* Go Fly!&#x20;

**Alternate Signup Methods**

* Another signup method is to sign up for the Auterion Suite directly from Auterion's website.&#x20;
* If you don't manually add vehicles, your Suite account won't have any registered.
* To add an aircraft to your account, you can use the aircraft serial number on the Vehicles page. However, please be aware that data sharing will be restricted until you physically connect your aircraft to a laptop and confirm that you have physical access to the drone.
* To register an aircraft that has been added by serial number, you need to follow these steps. First, connect the aircraft to a wifi network as described in the manual. Once connected, physically connect the aircraft to a computer and open a web browser. In the address bar, type in the IP address http://10.41.1.1. This will take you to a screen where you will see a large Register button. Click on this button and sign in to Auterion Suite to complete the registration process.

## Getting Data into the Suit

Aurora will automatically upload flight log files to the Suite with built-in wifi or LTE connections.

## Flight Logs

Aurora's autopilot has the capability to automatically create log files that record vital information about the aircraft's flight such as flight path, inputs received, and outputs sent, among others.&#x20;

These log files are stored on the onboard SD card. If the aircraft is registered in the Auterion Suite, Aurora will automatically upload the flight log files to the Suite when a wifi or LTE connection is available.

&#x20;Alternatively, logs can be downloaded to a PC. Flight logging starts when Aurora is armed and ends when Aurora is disarmed.

## Logs in the Suite

The easiest way to view the logs is with an [Auterion Suite account](https://suite.auterion.com/signup) (The basic version is free).

[Navigate to a particular flight](https://docs.auterion.com/public-documentation/vehicle-operation/auterion-suite-fleet-management/flights) to see many plots showing data such as angles, position, speed, GPS quality, vibration, etc. It will also show the build information, parameter values, and any errors detected in the flight.&#x20;

The suite enables the sharing of log files with the Camflite Support Team.

### Sharing Flight Logs with Support

To report a problem with a specific flight, activate the "Share with Manufacturer" option in Camflite.

## Logs without the Suite

If you cannot use the suite, you can download log files from Aurora to your PC using a USB connection.

### Downloading

Logs are stored in the onboard SD card in “[ulog](https://dev.px4.io/v1.9.0/en/log/ulog\_file\_format.html)” format. Use this procedure to download them.\
\
These are the requirements: Aurora drone, 1 SL8 battery, USB-C cable, and an Auterion Suite account. You can create a free account here, which is needed to download AMC PC.

|    |                                                    |
| -- | -------------------------------------------------- |
| 1. | Connect a USB cable from Aurora's IO panel to a PC |
| 2. | Install batteries to power Aurora                  |
| 3. | Open AMC PC and activate Advanced mode             |
| 4. | Navigate to "Analyze" menu, select "Log Download"  |
| 5. | Click "Refresh" to load the logs                   |
| 6. | Select desired files and click "Download"          |

### Viewing and Analysis

One of the simplest tools to use for analyzing ulog files is http://logs.px4.io. All you have to do is upload the file, and the tool will provide a detailed analysis of various data points, such as angles, position, speed, GPS quality, vibration, and more. It will also display software build information, parameter values, and any errors detected during the flight.

For other purposes, there are a variety of other [flight log analysis tools](https://docs.px4.io/v1.9.0/en/log/flight\_log\_analysis.html#analysis-tools). &#x20;



{% hint style="info" %}
Sharing aircraft logs with Camflite Support using the Auterion Suite is the simplest and fastest way to receive their assistance and have your Aurora back in the air after encountering any issue. You can do this by clicking on the "Share with the manufacturer" button.
{% endhint %}



## Privacy,  Data Sharing, and Security

Camflite and Auterion believe that the data generated by Aurora, such as flight logs, belongs to you. It is important that you have control over your data, feel confident about the security measures taken to protect it, and agree with how it is used.\
\
The Auterion Privacy Policy explains in simple terms how data can be transferred from Aurora to the Suite and to the partners of your choice.\
\
To elaborate, when Aurora is registered with a Suite account, you have the option to upload flight logs from the aircraft to Auterion servers automatically when an internet connection is available. You can access and review this data in your Suite account. Auterion employees cannot access your data. If you need to troubleshoot any issues related to a specific flight, you can share individual flight logs with Camflite Support through the Suite.

* Camflite and Auterion have designed a platform that prioritizes user privacy and full data control. The Aurora drone is equipped with hardware that supports both WIFI and LTE connections to the internet and other devices.&#x20;
* If you do not wish to use LTE, simply do not install a SIM card for data connection. Similarly, if you do not want the Aurora to connect to WIFI, you can avoid selecting any networks or providing passwords.&#x20;
* Additionally, you can disable WIFI on the pilot handset. To ensure maximum security, the user must have physical access/connection to the Aurora to register the aircraft to the Auterion Suite.&#x20;
* This is because the Auterion Suite allows for log uploads, live unit status tracking, live video streaming, and other important features.



