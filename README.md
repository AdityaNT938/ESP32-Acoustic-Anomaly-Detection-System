# 🎧 SmartEar: Edge-AI Acoustic Anomaly Detection System

## Overview

SmartEar is an AI-powered embedded system designed for **real-time industrial fault detection** using sound analysis.
It listens to machine acoustics and identifies early signs of failure, enabling **predictive maintenance** and improving safety.

This project combines **Digital Signal Processing (DSP)** and **Edge AI** to perform all computations locally on an ESP32 — eliminating the need for cloud processing.

---

##  Problem Statement

* Industrial machines generate complex, overlapping noise → faults are hard to detect
* Manual inspections are slow and inconsistent
* Cloud-based monitoring introduces latency and dependency
* Early fault signals are subtle and often missed

---

##  Objectives

* Develop a **Smart Acoustic Monitoring System** for fault detection
* Use **DSP techniques (Filtering, FFT, MFCC)** to process noisy signals
* Implement **Edge AI model on ESP32** (no cloud dependency)
* Enable **real-time anomaly detection with low latency**
* Ensure **low-cost and scalable deployment**

---

## System Architecture

```<img width="1500" height="583" alt="image" src="https://github.com/user-attachments/assets/f9285cca-61ab-47f3-8354-a7f2c3c02f84" />

```

---

##  Working Principle

1. Microphone captures machine sound as discrete signal
2. Signal is processed in frames using DSP techniques
3. **FFT** converts signal to frequency domain
4. **MFCC** extracts meaningful acoustic features
5. AI model classifies sound as:

   * ✅ Normal (Healthy Machine)
   * ❌ Anomalous (Fault Detected)
6. Alerts generated in real-time

## Circuit Diagram 

<img width="1266" height="614" alt="image" src="https://github.com/user-attachments/assets/5c23b855-114a-4d8c-aca7-cc93eab293f3" />


---

## Hardware Used

* ESP32 Microcontroller
* INMP441 MEMS Microphone
* USB Programming Interface

---

##  Software & Tools

* Arduino IDE
* ESP-IDF
* Edge Impulse Studio

---

##  DSP & AI Techniques

* Signal Filtering
* Fast Fourier Transform (FFT)
* MFCC (Mel Frequency Cepstral Coefficients)
* Machine Learning-based classification

---

##  Results & Performance

### 🔹 Model Performance

* Accuracy: **~85–92%**
* Inference Time: **4 ms**
* Processing Time: **561 ms**
* RAM Usage: **~12–18 KB**
  ### MFCC Feature Visualization
  <img width="692" height="581" alt="image" src="https://github.com/user-attachments/assets/2eb84ce6-911e-44a3-ab7b-c1f85e5501a9" />


### 🔹 Observations

* Normal signals form **dense clusters**
* Faulty signals show **irregular distribution**
* Stable MFCC patterns confirm proper DSP processing
* Real-world testing shows **high reliability**
  <img width="849" height="453" alt="image" src="https://github.com/user-attachments/assets/345ead46-5965-4b7a-bcd0-d4e02f69de08" />


---

## Testing

* Dataset-based validation
* Real motor testing in lab
* Mixed signal testing (Normal + Fault transitions)
<img width="713" height="333" alt="image" src="https://github.com/user-attachments/assets/ad6bfc04-91a7-4823-aeab-9403b1d2a6c4" />
<img width="526" height="405" alt="image" src="https://github.com/user-attachments/assets/c82c9f74-41e2-44fb-82fe-7a1d5fc14993" />



---

##  Key Features

*  Real-time anomaly detection
*  Fully offline (Edge AI)
*  Low-cost and scalable
*  Works in noisy industrial environments
*  Detects early-stage faults

---

##  Applications

* Predictive maintenance in industrial machines
* Smart factory monitoring systems
* Safety alerts in hazardous environments
* Home appliance health monitoring

---

---

##  Future Improvements

* Improve model accuracy using larger datasets
* Integrate wireless alert systems
* Add multi-machine classification
* Implement advanced deep learning models

---

##  Key Learning Outcomes

* Practical implementation of DSP (FFT, MFCC)
* Edge AI deployment on microcontrollers
* Real-time embedded system design
* Acoustic signal analysis

---

##  References

* Acoustic-Based Machine Condition Monitoring (MDPI, 2023)
* Sound-Based Predictive Maintenance Review (MDPI, 2025)
* Bearing Fault Diagnosis using ML (2023)

---


---

##  Conclusion

SmartEar demonstrates how **DSP + Edge AI** can transform traditional maintenance into a **smart, predictive, and efficient system**, reducing downtime and improving safety in industrial environments.

---


