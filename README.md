# 🚨 MQ135 Gas Sensor with Buzzer Alert (Analog Reading)

This project detects harmful gases in the air using the **MQ135 gas sensor** and triggers a **buzzer alarm** when gas concentration exceeds a preset level.  
It continuously monitors air quality through the sensor’s **analog output**, displays readings via the Serial Monitor, and provides an audible alert when the environment becomes unsafe.

---

## 🧠 Features

- Detects multiple gases (CO₂, NH₃, Benzene, Smoke, Alcohol, etc.)  
- Simple analog sensing – no complex calibration needed  
- Buzzer alert when gas concentration increases  
- Real-time readings on Serial Monitor  
- Works with Arduino UNO, Nano, or Mega  
- Easy to build, beginner-friendly  

---

## ⚙️ Components Required

| Component | Quantity | Description |
|------------|-----------|-------------|
| Arduino UNO | 1 | Microcontroller board |
| MQ135 Gas Sensor | 1 | Detects various air pollutants |
| Buzzer (Active) | 1 | Sounds alarm when gas detected |
| Jumper Wires | — | For connections |
| Breadboard | 1 | Optional for prototyping |
| USB Cable | 1 | For power and uploading code |

---

## 🔌 Circuit Connections

### 🔹 MQ135 Sensor → Arduino UNO
| MQ135 Pin | Arduino Pin |
|------------|-------------|
| VCC | 5V |
| GND | GND |
| A0 | A0 |

### 🔹 Buzzer → Arduino UNO
| Buzzer Pin | Arduino Pin |
|-------------|-------------|
| + (Positive) | D8 |
| - (Negative) | GND |

---

## ⚡ Power Supply

- Power the circuit via Arduino’s **USB port (5V)** or an **external 5V adapter**.  
- MQ135 requires a **5V supply** for accurate results.  
- Avoid powering the sensor directly from 3.3V sources.

---

## 🧩 Working Principle

1. **MQ135 sensor** measures the concentration of gases in the air and produces an analog output voltage.  
2. The **Arduino** reads this analog value from pin A0.  
3. If the sensor value exceeds the threshold, the **buzzer starts beeping**, signaling gas detection.  
4. Sensor readings and voltage are displayed on the **Serial Monitor**.  
5. The buzzer automatically turns off when gas concentration drops below the threshold.

---

## 🧪 Testing Procedure

1. Connect all components as per the circuit diagram.  
2. Upload the Arduino code (given below) using Arduino IDE.  
3. Open **Serial Monitor** (set baud rate to 9600).  
4. Observe live readings of sensor value and voltage.  
5. Bring a small amount of **smoke, alcohol, or LPG** near the MQ135 sensor (do not touch the sensor directly).  
6. When the value exceeds the defined threshold, you will hear the **buzzer alarm** and see “Gas Detected” printed on Serial Monitor.

---

## ⚙️ Calibration Tips

- Let the MQ135 **warm up for 1–2 minutes** before taking stable readings.  
- In clean air, the analog value should remain between **100–300**.  
- Adjust `GAS_THRESHOLD` in the code to a slightly higher value than your clean-air reading.  
- For higher precision, use advanced calibration formulas (optional).

---

## 🧰 Applications

- Indoor Air Quality Monitoring  
- Gas Leakage Detection  
- Smart Home Safety Systems  
- Environmental Sensing Projects  
- Educational Demonstrations  

---

## ⚠️ Safety Note

This project is meant for **educational and experimental purposes only**.  
The MQ135 sensor is **not a calibrated industrial-grade detector**.  
Do **not** use it as a primary safety device for gas leak detection or life-critical applications.

---

## 🧑‍💻 Author

**Project by:** Sourav Patel  
**Field:** Electronics & Robotics  
**Hardware:** Arduino UNO  
**Language:** C/C++ (Arduino IDE)

---
