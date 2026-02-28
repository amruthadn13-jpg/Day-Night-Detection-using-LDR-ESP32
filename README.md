# Day-Night-Detection-using-LDR-ESP32
**🌙 Day–Night Detection using LDR & ESP32 (Wokwi)**

This project uses an LDR (Light Dependent Resistor) module with an ESP32 to detect whether the environment is Dark or Light based on a fixed threshold value.

If the LDR analog value is less than or equal to 1000, the environment is considered Dark.
If the value is greater than 1000, it is considered Light.

The result is displayed on the Serial Monitor and an LED is used as an output indicator.

**🔧 Components Used**

ESP32

LDR sensor module (with AO pin)

LED

220Ω resistor

Jumper wires

Wokwi online simulator

**🔌 Connections**
LDR Module

VCC → 3.3V (ESP32)

GND → GND

AO → GPIO 14 (or any ESP32 ADC pin)

LED

LED anode → GPIO 18

LED cathode → GND through 220Ω resistor

**⚙️ Working Logic**

The ESP32 reads the analog value from the LDR using analogRead().

A threshold value is fixed as 1000.

Based on the sensor reading:

If value ≤ 1000 → Environment is Dark

If value > 1000 → Environment is Light

The LED turns ON in dark condition and turns OFF in light condition.

**🧠 Decision Rule**
If LDR value ≤ 1000  → Dark
If LDR value > 1000  → Light

**🧪 Example Output (Serial Monitor)**
LDR Value: 850
Environment is Dark

LDR Value: 2100
Environment is Light
**📌 Features**

Simple day and night detection

Real-time sensor reading

LED indication

Easy to simulate using Wokwi

**🚀 Applications**

Automatic street light system

Smart home lighting

Energy saving systems

Light-based automation projects

**📝 Note**

Only the AO (Analog Output) pin of the LDR module is used in this project.
The DO pin is not used, because we want to compare real sensor values using software.

**Author**
Amrutha D N
