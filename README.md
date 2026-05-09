# Smart-Wound-Monitoring-Band

## Overview
The Smart Wound Infection Monitoring Band is an IoT-based wearable healthcare system developed to continuously monitor wound conditions in diabetic patients, burn victims, and pressure ulcer patients. The system helps in early detection of infection by monitoring important wound parameters such as temperature, oxygen level, and wound color changes in real time.

---

## Problem Statement
Diabetic foot ulcers, pressure ulcers, and burn wounds are highly prone to infections that often remain unnoticed during the early stages. Current wound monitoring methods mainly depend on periodic manual inspection by healthcare professionals, which can delay infection detection.
Delayed identification of wound complications may lead to:
- Severe infections
- Tissue necrosis
- Increased hospitalization
- Amputations in critical cases
Patients require a continuous and non-invasive wound monitoring system that can provide real-time assessment and early warning of infection-related changes.

---

## Proposed Solution
This project proposes a wearable Smart Wound Infection Monitoring Band capable of continuously monitoring wound conditions using biosensors and IoT technology.

The system:
- Measures wound temperature
- Detects oxygen level variations
- Monitors wound color changes
- Performs trend analysis for infection detection
- Displays real-time wound data on a monitoring dashboard

The wearable design enables continuous patient monitoring outside hospital environments and supports early clinical intervention.

---

## Methodology Used

### 1. Thermal Sensing (IR-Based)
An IR-based temperature sensing mechanism is used to monitor wound temperature variations.
- Sensor Used: MLX90614
- Working Principle:
  The sensor detects infrared radiation emitted from the wound surface and converts it into temperature readings.
Temperature rise near the wound area may indicate inflammation or infection.

---

### 2. Oxygen Level Monitoring
The oxygen sensor monitors oxygen concentration near the wound area.
- Sensor Used: MAX30102
Reduced oxygen levels may indicate:
- Poor tissue healing
- Infection progression
- Reduced blood circulation

---

### 3. Bacterial Infection Detection Using UV Fluorescence
The system detects bacterial infection using UV-induced fluorescence analysis.
The bacterium *Pseudomonas aeruginosa*, commonly associated with infected wounds, produces fluorescent compounds that absorb ultraviolet (UV) light and emit a green fluorescence.
Methodology:
- A UV LED is used to illuminate the wound area.
- If *Pseudomonas aeruginosa* is present, the bacteria emit green fluorescent light.
- The emitted fluorescence is detected using the TCS34725 color sensor.
- The detected color variations help identify possible bacterial infection in the wound.
This method enables non-invasive and early-stage infection detection in wound monitoring applications.

---

### 4. IoT-Based Monitoring Using Blynk
The collected sensor data is processed using ESP32 and transmitted wirelessly to the Blynk IoT application for real-time wound monitoring.
The Blynk dashboard displays:
- Wound temperature readings
- Oxygen level values
- Infection-related sensor data
- Real-time monitoring updates
This enables continuous remote observation of wound conditions through a smartphone-based IoT platform.

---

## Results
The system successfully:
- Monitored wound temperature in real time
- Measured oxygen level variations
- Detected wound color changes
- Displayed trend analysis graphs for wound progression monitoring

The dashboard provided continuous visualization of wound parameters, helping in early infection detection.

---

## Applications
- Diabetic wound monitoring
- Burn wound monitoring
- Pressure ulcer assessment
- Remote patient monitoring
- Smart healthcare systems

