# I/O Board and Payload Power

The Input/Output (I/O) board, which is located at the bottom, acts as an interface between the Flight Management Unit (FMU) and various other components. It enables the FMU to access and control the rangefinder, nadir camera, and other similar devices, allowing for more efficient and accurate operation.

&#x20;

<figure><img src="../.gitbook/assets/69845348656--5FC579B3-8A5D-4457-9255-AFBFF1B8CC9A (1).jpg" alt="" width="375"><figcaption></figcaption></figure>





Onboard Power

Aurora has equipped the UAS with a 24v power source accessible through an XT30 connector at the bottom. The power supply is fed through a fused switching system and regulated by a linear regulator, ensuring clean and reliable power.



## I/O outputs

USB-C for webcam, flash storage, etc

**Telem1**- UART4 and I2C from FMU

**Ethernet**- for camera or other network-based payloads

**Cap**- FMU CH 7 and CH 8, FMU CAP, and one GPIO from MC

**Can1**- CAN from FMU

**PWM**- ch7-8





<div align="center">

<figure><img src="../.gitbook/assets/can.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/cap.png" alt=""><figcaption></figcaption></figure>

</div>



<div>

<figure><img src="../.gitbook/assets/eth.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/gps.png" alt=""><figcaption></figcaption></figure>

</div>



## Payload Connector

<div align="left">

<figure><img src="../.gitbook/assets/Screenshot 2023-12-27 032435.png" alt="" width="231"><figcaption><p>Payload Pinouts</p></figcaption></figure>

</div>

## USB-C FMU Plug

The Aurora drone features an exclusive USB port that is situated at the bottom of the device. This USB port is dedicated to direct connection to the onboard mission computer, which manages and coordinates the drone's operation. With this USB port, you can comfortably perform essential tasks such as upgrading the drone's firmware and communicating with the Flight Management Unit (FMU).To establish a connection with the flight computer, it is essential to power up the Aurora device as the USB port alone does not provide any power. Thus, you will need to ensure that the Aurora device is powered on before attempting to communicate with the flight computer.
