# Herelink Pilot Controller

## Herelink

Aurora ships with the Herelink system. Here is the [CubePilot documentation](https://docs.cubepilot.org/user-guides/herelink/herelink-overview). Below are a few points specific to usage with Aurora.

### Hardware Controls







### Mission Control GUI

Herelink ships with the Auterion Mission Control (AMC) app installed. Details of the GUI are in the AMC section of the wiki.

### Setup

To change the color scheme, go to AMC > Settings and select either Outdoor (white background) or Indoor (black background). To adjust screen brightness or audio volume, swipe down from the top of the screen to access Android settings. For optimal viewing, we recommend setting the brightness and volume to their highest levels.

### Antennas

For optimal performance, it is recommended to position the whip antenna in a vertically upward direction and ensure that the top surface of the disc patch antenna is facing toward Aurora.

### Charging

For the device to charge properly, it requires a minimum of 2 amps of current. Inadequate current may result in slow charging or loss of charge. To achieve optimal performance, we suggest using an external power supply to keep the radio fully charged.

### WiFi



<figure><img src="../.gitbook/assets/Screenshot 2023-07-02 185335.png" alt=""><figcaption></figcaption></figure>

#### Internet

To connect Herelink to the internet, you can establish a wifi connection. This feature enables you to download satellite maps for offline utilization. Here are the steps to follow for a successful connection:

\
1\. Swipe down from the top of the touch screen.\
2\. Press and hold the Wifi button (as seen in the picture).\
3\. Select your wifi network and enter the password if prompted.&#x20;

\
If you have the correct information and a functioning wifi access point, you should now be connected to the internet on Herelink.



{% hint style="info" %}
Herelink can only connect to 5 GHz networks. The 2.4 GHz band is used for communication with the aircraft.
{% endhint %}

{% hint style="info" %}
Activate 5 GHz wifi hotspot on iPhone 12: Settings > Personal Hotspot > Maximize compatibility: Disable. iPhone 11 and older do not offer a 5 GHz wifi hotspot.
{% endhint %}

By using Herelink, you can easily set up a Wi-Fi network and connect your iPad or PC to Aurora while in flight. This will allow you to utilize AMC or other companion apps such as ESRI Site Scan.



{% hint style="info" %}
To establish in-flight connections, we suggest using the Herelink hotspot discussed in this section as Aurora's onboard wifi chip has limited range. It's important to note that the onboard wifi is disabled for RID.
{% endhint %}

{% hint style="warning" %}
To avoid consuming too much power, it's best to connect the Herelink to a power source while using the hotspot. This is a precautionary measure that is highly recommended.
{% endhint %}

<table><thead><tr><th width="150">Device</th><th>Action</th></tr></thead><tbody><tr><td>Herelink</td><td>Power on and open AMC on the Herelink controller.</td></tr><tr><td>PC</td><td>Power on and open <a href="https://suite.auterion.com/downloads">AMC PC </a>on your computer. </td></tr><tr><td>Herelink</td><td>Hotspot settings (first time): <br>Pull down from the top of the touch screen two times. Tap <strong>and hold</strong> the hotspot icon <img src="broken-reference" alt="" data-size="line"> in the top-right. Select Tethering &#x26; Portable Hotspot. </td></tr><tr><td>Herelink</td><td>Enable hotspot: <br>Pull down from the top of the touch screen two times. Tap the hotspot icon <img src="broken-reference" alt="" data-size="line"> in the top-right.</td></tr><tr><td>PC</td><td>Connect to the Herelink wifi network (named something like “Android…” or “DV...”) if AMC PC does not recognize the aircraft, set up a UDP Link. </td></tr></tbody></table>

#### UDP Link

If you're still unable to connect despite following the previous steps, try setting up a new UDP link on your laptop or tablet. Simply tap on the AMC icon located in the top-left corner and navigate to the settings>comm links section to create a new UDP Link. Make sure to enter the necessary settings as indicated below:



<figure><img src="../.gitbook/assets/spaces_8dwrGJhxGd9cIvsStziq_uploads_dHMaZomIQrRkPZ7EnE5i_Screenshot from 2022-04-04 12-27-31.webp" alt=""><figcaption></figcaption></figure>

To connect your configuration, select it from the list and hit the "Connect" button. You can also set it up to connect automatically when you start up. It's crucial to make sure your device receives at least 2 amps of current for proper charging. Inadequate current could lead to slow charging or loss of charge.

**We recommend using an external power source to keep the radio fully charged for optimal performance**. To establish a new UDP link on your laptop or tablet, tap on the AMC icon in the top-left corner and navigate to settings>comm links. Create a new UDP link from there, and provide all the necessary settings, as shown below. Make sure that the "IRE" is set to "WIRED," and that the uplink rate is non-zero.

* Open the AMC app on Herelink Pilot Handset and verify the connection to the aircraft.&#x20;
* Power off Aurora and, optionally, the Herelink Pilot controller.
* Replace the Herelink Cover.

{% hint style="info" %}
Please note that it is not possible to connect Aurora with multiple Herelinks. Attempting to connect an additional remote will result in disconnection from the previous one, even if the second remote is powered off.
{% endhint %}
