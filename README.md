# ESC_RPM_TIVA
ESC control and RPM measurement through TM4C123GH6PM.

# ESC Control and RPM Measurement using TM4C123

### Author: Fida Hussain  
**University of Engineering and Technology (UET), Lahore**  
**5th Semester - Mechatronics Engineering**

---

## 📘 Overview
This project controls a **BLDC motor** via an **Electronic Speed Controller (ESC)** using the **TM4C123 (Tiva C Series)** microcontroller. It generates a 50Hz PWM signal, reads analog throttle input, and measures RPM via an optocoupler.

---

## ⚙️ Features
- 50Hz PWM generation using Timer0A and Timer1A  
- ESC arming and throttle control (1000–2000 µs pulse)  
- RPM measurement using GPIO interrupt and Timer2A  
- Analog input from potentiometer (PE3/AIN0)  
- Live RPM display via UART0 (9600 baud)

---

## 📂 File Structure
ESC_RPM_TIVA/
├── src/ → Source files (.c)
├── inc/ → Header files (.h)
├── README.md


---

## 🧩 Hardware Connections
| Signal | Pin | Description |
|--------|-----|-------------|
| PWM Output | PB6 | ESC control signal |
| RPM Sensor | PB2 | Optocoupler input |
| ADC Input | PE3 | Potentiometer |
| UART Tx/Rx | PA0/PA1 | Serial communication |

---

## 🛠️ Tools Used
- **Keil µVision** for Embedded C programming  
- **TM4C123GH6PM (Tiva C Series)** microcontroller  
- **UART Serial Terminal (9600 baud)**  
- **Optocoupler + BLDC + ESC + Potentiometer**

---

## 📈 Future Improvements
- Implement PID control for stable speed regulation  
- Add LCD display for RPM  
- Enable remote throttle control (via Bluetooth or Wi-Fi)

---
