---
menu: Operating HealthyPi v4
parent: getting-started.md
weight: 2
---

## Operating HealthyPi v4

### Connecting sensors

#### Connecting the ECG/Respiration Electrodes

A 3-electrode cable along with a standard stereo jack is provided along with the shield to connect the electrodes to the  board.
The other side of the electrode connector would connect to snap-on electrodes attached to the body. For testing purposes, you can use an ECG simulator to provide inputs to the board.

![Open the terminal](images/hpi4-connect-ecg.jpg)

**Important Warning:**
When connecting the electrodes to the body, it is safer to disconnect the mains power source to the Arduino. For example, if  you are using the Arduino along with a laptop, disconnecting the battery charger from the laptop would be a safe option.

Place the electrodes on the body in these positions to get the best signal. However, placing it in other positions on the chest would work as well with differing ECG signal patterns. For getting respiration using the [Impedance Pneumography](http://www.ti.com/lit/an/sbaa181/sbaa181.pdf), it's best to wear them on the chest as given in the figure below to get the best signal.

![Wearing the Electrode](images/connecting electrodes.png)

#### Connecting the Pulse Oximetry Probe

[Pulse oximetry](https://en.wikipedia.org/wiki/Pulse_oximetry) is an optical method of non-invasively measuring the oxygen content in the blood. This is achieved with the help of a finger-clip probe that contains some LEDs on one side of the clip and a photo-detector on the other side.

The LEDs emit light in the red and IR wavelengths. Some of these are absorbed by the blood and the rest is transmitted through to the other side of  the finger, which is is picked up by the photo-detector. The Pulse Oximetry front-end measures this variance in the transmitted light intensity to display the [Photoplethysmogram (PPG)](https://en.wikipedia.org/wiki/Photoplethysmogram) signal. SpO2 is a computed value derived from the Red and IR PPG signal.

To start measuring, simply plug-in the provided SpO2 finger-clip probe to the DB9 connector on the HealthyPi v4 board. If the probe is properly plugged in, you should see a Red glow inside the probe.

[Photo of plugging in the DB9 connector]

#### Connecting the temperature sensor

A digital human body temperature sensor based on the MAX30205 from Maxim Integrated is provided. This sensor provides direct, calibrated temperature values over a digital I2C interface. The sensor comes as qwiic based connectors making the interface even more simpler than before and a cable for maximum flexibility.

![Temperature sensor](images/hpi3-temperature.jpg)

No more colour coding confusion, Just Plug the qwiic based temperature sensor directly to read data.Refer the connection shown in the following picture.

[Photo of temperature sensor connector with color codes]

### Selecting modes

#### Explore with two modes

Now switching between two different modes in the HealthyPi v4 is  made simple. You have to just slide the mode selection switch to experience the features hidden under the two modes, the default mode will be HPi3 mode and another is the wearable mode.Check out the below video for mode selection tutorial.

#### Choice for connectivity

In the wearable mode the HealthyPi v4 acts as wireless, you can choose the default BLE mode or enter Webserver mode using the on-board push button. Stream live real-time vitals in your smart devices with these communication protocols. Check out the below video for HealthyPi v4 wireless connectivity tutorial.    

### Powering the device

#### Plugging Battery

Powering the device with a LiPo rechargeable battery improves its portability. HealthyPi v4 can be used as a standalone device, without external interfaces or power.The battery can be directly connected to HealthyPi v4 through the onboard 2-pin JST-PH connector.Check out the image below connecting the battery with HealthyPi v4.

#### Using a USB Port

You can plug cables into a USB port in HealthyPi v4 at any time regardless of whether the device is powered on or off.The USB port can be used for powering the device, uploading the code and charging the battery.Check out the image below showing the USB connection.

### On-board Indication