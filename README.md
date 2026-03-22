# HexDigit-EMG-Controlled-Wearable-Third-Thumb
---
## **The reason behind doing this project?**

The idea behind this project was to explore human augmentation using accessible hardware. I wanted to go beyond traditional robotics and build something that directly interfaces with the human body — where muscle intent translates into mechanical action in real time.

Instead of using buttons or switches, the goal was to use EMG (Electromyography) signals from the pectoral muscle to control a wearable robotic thumb. This creates a more natural and intuitive interaction, making the device feel like an extension of the body rather than an external tool.

Additionally, I wanted to challenge myself by combining multiple domains:

* Bio-signal processing
* Wearable electronics
* Soft robotics (TPU flexure design)
* Tendon-driven actuation

---

## **Is it solving a real-life problem?**

Yes — the system demonstrates a low-cost approach to human augmentation and assistive technology.

Potential real-world applications include:

* Assistive devices for individuals with reduced hand mobility
* Prosthetic control systems using EMG signals
* Industrial assistance (third hand for holding tools/components)
* Rehabilitation and physiotherapy devices
* Human-machine interfaces for robotics and control systems

Even in its current form, the device acts as a functional “third hand,” capable of stabilizing objects like tools while the user performs other tasks.

---

## **Materials Required:**

* BioAmp EXG Pill (Upside Down Labs)
* Arduino Nano
* MG995 Servo Motor
* XY3606 Buck Converter
* 11.1V (3S) Li-ion Battery (with BMS)
* Nylon Fishing Line (0.6 mm, high tensile strength)
* PTFE Tube (for tendon routing)
* 3D Printed TPU Thumb (flexure-based design)
* Velcro Straps (50 mm) for mounting
* 1000µF Capacitor (for servo stability)
* Rocker Switch
* DC Connectors (Male/Female)
* Wires (20–22 AWG)
* Heat shrink, connectors, mounting hardware

---

## **Procedure:**

### **1. EMG Signal Acquisition**

* Electrodes were placed on the medial region of the pectoralis major for strong EMG signals.
* The BioAmp EXG Pill was used to capture and amplify the signal.
* EMG-only mode was enabled for cleaner readings.

---

### **2. Signal Processing and Control**

* The amplified EMG signal was read using the Arduino Nano (analog input).
* Envelope detection and filtering were applied in code.
* A threshold-based trigger system was implemented:

  * Muscle flex → thumb closes
  * Relax → thumb opens

---

### **3. Mechanical Design (Thumb)**

* The thumb was redesigned as a **single-piece TPU flexure structure**.
* This eliminated the need for rigid joints and rubber bands.
* The design allows natural curling toward the palm.

---

### **4. Tendon-Driven Actuation**

* Nylon fishing line was used as a tendon.
* A PTFE tube was used to guide the tendon and reduce friction.
* The tendon is routed from the thumb to the servo mounted on the forearm.

---

### **5. Actuator Module (Forearm Mount)**

* MG995 servo was mounted on a 3D-printed forearm bracket.
* A custom spool was designed to wind the tendon smoothly.
* Velcro straps were used for wearable mounting.

---

### **6. Power System**

* A 3S (11.1V) battery powers the system.
* XY3606 buck converter steps voltage down to ~5.5V.
* A capacitor stabilizes servo current spikes.

---

### **7. Integration and Testing**

* System was tested incrementally:

  * Servo control via serial
  * Tendon movement calibration
  * EMG signal tuning
* Final system achieved:

  * Instant response
  * No false triggers
  * Natural thumb movement

---

### **Demo Highlights:**

* Muscle-controlled thumb actuation
* Real-time response with no perceptible delay
* Ability to hold and stabilize tools (e.g., screwdriver)
* Natural curling motion toward the palm



https://github.com/user-attachments/assets/0a5c212e-0fbb-423b-883d-19cf708ce9a1



https://github.com/user-attachments/assets/ec5b03b5-4215-40a0-b7c8-aad188f1114d


---

