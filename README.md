# 💧 Water Level Monitoring and Pump Control System

This project is a *microproject* developed as part of the *S3 Electronics and Computer Engineering* course at *Saintgits College of Engineering*.  
It aims to design an *automatic water level monitoring and pump control system* using an *ESP8266 (NodeMCU)* and an *ultrasonic sensor* to prevent water wastage and pump dry-run conditions.

---

## 🧠 Project Overview

Manual control of water pumps often leads to problems such as *tank overflow, **underflow, and **unnecessary power usage*.  
This project provides a smart solution by automatically monitoring water levels and controlling the pump accordingly.

The system:
- Monitors the water level in an overhead tank using an *ultrasonic sensor*
- Automatically turns the *pump ON* when the level is *LOW*
- Turns *pump OFF* when the tank is *FULL*
- Protects the pump from *dry-run* operation

---

## ⚙ Components Used

| Component | Quantity | Description |
|------------|-----------|-------------|
| ESP8266 (NodeMCU) | 1 | Microcontroller board |
| Ultrasonic Sensor (HC-SR04) | 1 | Measures tank water level |
| Relay Module | 1 | Controls the water pump |
| Water Pump | 1 | DC/AC motor pump |
| Jumper Wires | - | For circuit connections |
| Power Supply | 1 | 5V or USB power |

---

## 🔌 Circuit Connections

| Ultrasonic Sensor | NodeMCU Pin |
|--------------------|-------------|
| VCC | VIN (5V) |
| GND | GND |
| TRIG | D5 |
| ECHO | D6 |

| Relay Module | NodeMCU Pin |
|---------------|-------------|
| VCC | 3.3V / 5V |
| GND | GND |
| IN | D4 |

---

## 📊 Working Principle

1. The *ultrasonic sensor* continuously measures the distance from the sensor to the water surface.  
2. Based on the distance, the *ESP8266* determines whether the tank is full, mid, or low.  
3. If the level is *low, the **relay activates* and turns ON the pump.  
4. When the level reaches *full, the **relay deactivates*, turning OFF the pump.  
5. This ensures optimal use of water and electricity.

---

## 💻 Code

The complete source code is provided in the file:  
[water_leveloriginal.ino](./water_leveloriginal.ino)

Upload the code to your *NodeMCU* using the *Arduino IDE* after connecting all components as per the circuit.

---

## 🖼 Block Diagram

Include your block diagram in the repository under:

![Block Diagram](images/block_diagram.png)!![WhatsApp Image 2025-10-20 at 11 51 24_e6d2ce97](https://github.com/user-attachments/assets/88b6694f-74af-42eb-822a-94672ab15a06)

Then reference it like this:

![Circuit Diagram](images/circuit_diagram.png)![WhatsApp Image 2025-10-17 at 11 13 14_6f22a536](https://github.com/user-attachments/assets/93062475-d184-4576-8c9f-0598948a7945)


---

## 🎥 Demonstration Video

Upload your project demo video to *Google Drive, **YouTube, or **GitHub Releases*, and link it below:

🔗 [Watch Demonstration Video]





https://github.com/user-attachments/assets/7dbe265c-3b78-4a49-8d84-f4f4a56a1834



(Replace with your actual video link)

---

## 📄 Project Report

You can include your detailed report as a PDF 

📘 [Download Project Report (PDF)](./Water_Level[WATER_LEVEL_MONITORING_MICROPROJECT (4).pdf](https://github.com/user-attachments/files/22996250/WATER_LEVEL_MONITORING_MICROPROJECT.4.pdf)
_Report.pdf)





---

## 🚀 Future Enhancements

- Add *IoT-based monitoring (Blynk / ThingSpeak)*  
- Include *buzzer alerts* for dry-run or overflow  
- Add a *manual/auto switch* for flexibility  
- Integrate *battery backup* for uninterrupted control  

---

## 👩‍💻 Author

*Anita Susan Thomas*  
S3 Electronics and Computer Engineering  
Batch 2024–2028  
*Saintgits College of Engineering*

---

## 📝 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🏫 Acknowledgement

This project was developed as part of the *Microproject Submission* for the  
*Department of Electronics and Computer Engineering*,  
*Saintgits College of Engineering*, Kottayam.

---

## 📷 Project Setup

You can include your setup image here for visual reference:

![Project Setup](images/project_setup.jpg)

