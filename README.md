# Arduino Parking Sensor
Making a Parking Sensor with Arduino is Actually Very Simple. You can make it yourself using the following materials

This Content Also Has A YouTube Video! Don't Forget to Watch! [Code Chain](https://www.youtube.com/@CodeChain) [Video](https://youtu.be/QbnlMhDsDws)

# What is HC-SR04 Ultrasonic Distance Sensor?
Designed for use in development boards such as Arduino, this sensor is a distance measurement sensor used in most robotic projects due to its cheapness and ease of use.

According to the information given by the manufacturer, this sensor can measure between 2 cm and 400 cm with a margin of error of 1%. But if we talk by looking at the user experiences, the most efficient measurement distance is between 2 – 200 cm.

# HC-SR04 Ultrasonic Distance Sensor Features And Pinouts
> Technicial Specifications

Features | Outputs 
--- | --- 
**Operating voltage** | DC 5V 
**Working Current** | 15mA
**Operating Frequency** | 40KHz
**Maximum Measurement** | 4m
**Minimum Measurement** | 2cm
**Measuring Range** | 3mm
**Measuring Angle** | 15 degree
**Trigger Input Signal** | 10µS TTL
**Dimension** | 45 x 20 x 15 mm

# HC-SR04 Ultrasonic Sensor Connection

<img src="https://github.com/musarda/Arduino-Parking-Sensor/blob/main/img/HC-SR04.png" title="HC-SR04" alt="HC-SR04" width="250">

- **VCC** : It is the power supply for the HC-SR04 Ultrasonic distance sensor, which we connect 5V pin to Arduino.
- **Trig** : The (Trigger) pin is used to trigger ultrasonic audio signals.
- **Echo** : pin generates a BPM when the reflected signal is received. The pulse length is proportional to the time it takes to detect the transmitted signal.
- **GND** : It must be connected to Arduino grounds.

# Working Principle of Distance Sensor

The working principle of the HC-SR04 sensor is as follows;

The signal applied from the Trig pin of the sensor provides an **ultrasonic** sound emission at a frequency of 40 kHz. When this sound wave hits any object and returns to the sensor, the Echo pin becomes active. By measuring the time between these two signals, that is, by detecting the echo of the sound, we can determine the distance of the object from the sensor.

# Using HC-SR04 Ultrasonic Distance Sensor with Arduino

Now that we understand the working principle of the ultrasonic distance sensor, we can make a sample project with Arduino.

Connecting the HC-SR04 to Arduino is quite easy. I recommend placing the sensor on your breadboard. Because in the case of a minor contact, your sensor will not provide accurate data.

# Necessary materials
- 1x Arduino UNO
- 1x Breadboard
- 1x HC-SR04 ultrasonic distance sensor
- 1x Buzzer
- 1x 330Ω Resistance
- Jumper cable

# Connection Diagram

![Circuit_Diagram](https://github.com/musarda/Arduino-Parking-Sensor/blob/main/img/Circuit_Diagram.jpg)

> Connect the VCC pin to the 5V pin on the Arduino and the GND pin to the Ground pin on the Arduino as seen in the circuit diagram above.
  Connect the trig pin to the 7th digital pin of the Arduino and the echo pin to the 6th digital pin of the Arduino.
