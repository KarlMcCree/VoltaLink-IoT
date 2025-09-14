**VoltaLink: High-Power AC IoT Timer GenAI Board.**

VoltaLink is a professional, safety-oriented IoT development board which allows voice and manual control of high-power appliances (up to 30A at 220 V/110 V) using high-power AC. It is designed based on ESP32 and connects easily with Google Home, Alexa, and Siri to be used as a smart home automation device and offers powerful local control.

🚀 Key Features
⚡ High-Power Control: Switches AC loads as large as 30A with a high-resilience industrial-grade relay safely.

🗣️ Voice Assistant Integration: Complete integration with Google Assistant, Amazon Alexa, and Apple Siri through internet of things cloud services.

🤖 Manual & Local Control: Tactile button and web interface independent of cloud functioning.

🔒 Built-in Safety:

Galvanic Isolation: Hi-Link AC/DC converter isolates high and low voltage circuits.

Fused AC Input: Has fuse protection screw terminal.

Flyback Diode and TVS Protection: Guards sensitive circuits against voltage spikes.

🌐 Web Interface: Local web interface with simple scheduler of timer controls and manual override.

📊 Expansion Ready: I2C (e.g., with an OLED display), UART, and other additional GPIOs breakout headers.

🛠️ Technical Specifications
Parameter	Specification:
Microcontroller:	ESP32-WROOM-32D
WiFi Connectivity:	802.11 b/g/n (2.4 GHz)
Input Voltage:	110V / 220V AC (50/60 Hz)
Output Rating:	30A Max, 250V AC
Low-Voltage Logic:	3.3V & 5V DC
Control Interfaces: Voice, Web Server, Physical Button
Safety Features: Fuse, Optoisolation, Flyback Diode, Creepage/Clearance.
Design Software:	KiCad 7

📸 Hardware Overview

The PCB has been done in such a way that there is a distinct separation between a High-Voltage (right) and Low-Voltage (left) segment, which is done to be safe.

AC Input/Output Terminal Blocks: Safe connections of mains wiring.

Fuse Holder: To protect against over-current.

HLK-PM05 Hi-Link Module: 220 VAC to 5 VDC power supply is isolated.

ESP32-WROOM-32D: WiFi and control logic system-on-chip.

Industrial Relay (RAYEX-L90): 30A switching.

Optoisolator (PC817): Signal isolates the relay driver.

Manual Control Button: To set a local timer and override.

Status LED & Buzzer: To provide feedback to the user.

I2C Header: To be able to connect an OLED display or other sensors.

⚙️ Software & Firmware
The firmware is based on the Arduino Core of the ESP32 and it offers:

Web Configuration Portal: This enables the timing through any web browser.

Network Time Protocol (NTP) Sync: Synchronous timekeeping of schedules.

EEPROM Storage: Storing timer settings on power ups.

RESTful API: To be able to integrate with other smart homes.

🛡️ Safety Warning
⚠️ HIGH VOLTAGE WARNING ⚠️

In this project, one will work with LETHAL MAINS VOLTAGE(110 V/ 220 V AC). The circuit should not be attempted to be constructed or operated by anyone but a qualified person who has knowledge of the hazards and of the precautions which are required. Always:

Work de-energized. Do not solder or alter the board when it is plugged.

Use a proper enclosure. The board assembled should be in a completely insulated non-conducting enclosure.

Ensure proper grounding.

Test cautiously. Initial testing should be done by using a current-limited power supply and GFCI outlet.

🧩 Future Enhancements
CT sensors energy monitoring.

Bluetooth Low Energy (BLE) provisioning.

Over-the-Air (OTA) updates.

Thermal protecting PCB-mount temperature sensor.

4 Layer board schematics and layout to improve its EMC performance.

👥 Contributing
Donations, bugs and proposals are also welcome!.
