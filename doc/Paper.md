# M5Stack NanoC6 Thread Matter

## ESP32-C6

The ESP32-C6 is a microcontroller with wireless communication functionality that supports Wi-Fi6 (2.4GHz), Thread, Zigbee, and Bluetooth5.
ESP-IDF, a software development environment provided by Espressif, enables the development of software for devices that use the aforementioned wireless communication functions.
ESP-IDF is a microcontroller with wireless communication functionality that supports ESP-IDF, Bluetooth5, and ESPressif's software development environment.
Espressif also provides esp-matter as a development environment for Matter devices using its own devices.
Using esp-matter, you can develop software for the ESP32-C
With esp-matter, you can create Matter devices that connect via Wi-Fi or Thread using the ESP32-C6.

## M5Stack NanoC6
The NanoC6 is an ESP32-C6-based wireless communication unit manufactured and sold by M5Stack:
 - small 24x13x10mm^3 unit with wireless communication function.
 - contains the ESP32-C6, a USB Type-C connector, power circuitry, GROVE-compatible connectors, and a color LCD display, GROVE-compatible connectors, color LEDs, and a push-button.

It can be used to prototype devices utilizing Wi-Fi, Thread, Bluetooth5, and Zigbee in a single unit.

## Thread Matter Contact Sensor

**Thread Matter Contact Sensor device using the NanoC6**

Using the NanoC6 and some expansion units, we configure a Thread Matter device that acts as a Contact Sensor.
Instead of a regular Contact Sensor, connect a pushbutton to the NanoC6 and use it as a Contact Sensor.
The button is open when it is released and closed when it is pressed.

## OpenThread Border Router (OTBR)
Border Router (OTBR) is a device that relays devices communicating via Thread to devices communicating via Wi-Fi or Ethernet.

A device that relays devices communicating via Thread to devices communicating via Wi-Fi or Ethernet is called a Border Router.
OpenThread is an implementation of the Thread communication stack.

and includes a Border Router implementation, OpenThread Border Router
(The ESP32 development environment, ESP-IDF, includes

ESP-IDF includes an implementation of OTBR for the ESP32 series, which can be configured and written for NanoC6
The ESP-IDF includes an OTBR implementation for the ESP32 series, which works simply by building and writing the configuration for the NanoC6.

If you have a Thread border router, this is not necessary.
If you do not have a Thread border router, you will need to build OTBR on NanoC6.

## Setup
- Write a `NanoC6 OpenThread Border Router (Single NanoC6)` firmware to the first NanoC6.
- `NanoC6 Thread Matter Contact Sensor` is written to the second NanoC6.

