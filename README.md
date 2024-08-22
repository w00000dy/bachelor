# Web Bluetooth Remote Control

With this project you can control your smartphone from a browser via Bluetooth.

## How it works
Since the Web Bluetooth API is currently an experimental technology, and the browser cannot act as a HID due to API restrictions, we don't use it. Instead, we use an ESP32 D1 Mini NodeMCU. The ESP32 supports Bluetooth LE 4.2 and allows us to act as a \ac{HID} device. The ESP32 then communicates with the browser via UART using the Web Serial API.

![Experiment Design](https://github.com/user-attachments/assets/bf531d0b-fa89-40dd-878e-cfb95e12c3ea)

