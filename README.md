**⚡ AC Clamp Meter**

A KiCad-based PCB design for a non-invasive AC measurement device using a Current Transformer (CT) sensor. Built as part of an EEE hardware project.
_____________________________________________________________
**📌 Overview**

This project implements an **AC Clamp Meter** circuit that measures alternating current without breaking the circuit. The design uses a split-core CT sensor, a signal conditioning front-end, and outputs a calibrated voltage proportional to the measured current.
---------------------------------------------------------------------------------------
|                Parameter              |                     Value                   |
|---------------------------------------|---------------------------------------------|
| Measurement Range                     |     0 – 110A AC (adjustable)                |
| CT Sensor                             |    SCT-013 / YHDC (30A or 100A variant)     |
| Output                                |          0–3.3V analog (ADC-ready)          |
| PCB Tool                              |                  KiCad 7.x                  |
---------------------------------------------------------------------------------------
______________________________________________________________
**🔌 How It Works**

CT Sensor (clamp)
      │
      ▼
3.5mm Jack Input
      │
      ▼
Signal Conditioning
(R1, R2, R3, R4 + D12 + C1)
      │
      ▼
Arduino Nano ADC Pin
      │
      ▼
Firmware Processing
      │
      ▼
I2C OLED Display
(GND / VCC / SDA / SCL)

__________________________________________________________________
