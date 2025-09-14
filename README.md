#  VoltaLink: High-Power AC IoT Timer GenAI Board

**VoltaLink** is a professional, safety-oriented IoT development board that enables **voice** and **manual control** of high-power appliances (up to **30A at 220V/110V**) using AC mains.  
Built on the **ESP32**, VoltaLink connects seamlessly with **Google Home, Alexa, and Siri** for smart home automation, while also offering **local web-based control**.

---

##  Key Features

-  **High-Power Control** – Switches AC loads up to **30A** with an industrial-grade relay safely.  
-  **Voice Assistant Integration** – Works with **Google Assistant, Alexa, Siri** via IoT cloud services.  
-  **Manual & Local Control** – Tactile button + local web interface, independent of the cloud.  
-  **Built-in Safety**:  
  - Galvanic Isolation with Hi-Link AC/DC module.  
  - Fused AC input with protection terminal.  
  - Flyback diode & TVS protection.  

-  **Web Interface** – Simple timer scheduler & manual override.  
-  **Expansion Ready** – I²C, UART, and GPIO headers for sensors or displays.  

---

##  Technical Specifications

| Parameter              | Specification                     |
|-------------------------|-----------------------------------|
| **Microcontroller**     | ESP32-WROOM-32D                  |
| **WiFi Connectivity**   | 802.11 b/g/n (2.4 GHz)           |
| **Input Voltage**       | 110V / 220V AC (50/60 Hz)        |
| **Output Rating**       | 30A Max, 250V AC                 |
| **Low-Voltage Logic**   | 3.3V & 5V DC                     |
| **Control Interfaces**  | Voice, Web Server, Physical Btn  |
| **Safety Features**     | Fuse, Optoisolation, Flyback, Creepage Clearance |
| **Design Software**     | KiCad 7                          |

---

##  Hardware Overview

The PCB is carefully designed with **high-voltage (right)** and **low-voltage (left)** separation for safety.  

- **AC Terminal Blocks** – Safe connection of mains wiring.  
- **Fuse Holder** – Over-current protection.  
- **Hi-Link HLK-PM05** – Isolated 220V → 5V power supply.  
- **ESP32-WROOM-32D** – Core WiFi + control logic.  
- **Industrial Relay (RAYEX-L90)** – 30A switching.  
- **Optoisolator (PC817)** – Isolation between control & relay.  
- **Manual Button** – Local timer & override control.  
- **LED + Buzzer** – User feedback indicators.  
- **I²C Header** – Expansion for OLED display or sensors.  

---

##  Software & Firmware

The firmware is built on the **Arduino Core for ESP32** and provides:

-  **Web Configuration Portal** – Configure timers via browser.  
-  **NTP Sync** – Automatic time synchronization.  
-  **EEPROM Storage** – Saves timer schedules across reboots.  
- 🔗 **RESTful API** – Integrates with external smart home systems.  

---

##  Safety Warning  

⚠️ **HIGH VOLTAGE NOTICE** ⚠️  

This project works with **LETHAL MAINS VOLTAGE (110V/220V AC)**.  
**Do NOT attempt** unless you are qualified and aware of the safety precautions.  

**Always follow these rules:**  
-  Work **de-energized** – Never solder/test while powered.  
-  Use a **proper insulated enclosure**.  
-  Ensure **proper grounding**.  
-  Test with **GFCI outlets** and current-limited supply.  

---

##  Future Enhancements

-  CT sensor integration for **energy monitoring**.  
-  **BLE provisioning** for easy setup.  
-  **OTA firmware updates**.  
-  PCB-mount **temperature sensor** for thermal protection.  
-  **4-layer board** design for improved EMC performance.  

---

##  Contributing

Pull requests, issues, and feature suggestions are welcome!  
Donations to support the development are also appreciated.  

---

##  License  

This project is released for **educational purposes only**.  
⚠️ Use at your own risk when working with mains power.  

