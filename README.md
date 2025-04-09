# 📡 ESP32 Modular Datalogger

A robust and modular data acquisition system based on ESP32 and Arduino Pro Mini, designed to collect and transmit real-time sensor data to the cloud. Built for flexible use in agricultural, environmental, and industrial automation applications.

---

## 📌 Features

- **Modular Architecture**: Combines ESP32 and Arduino Pro Mini to expand IO capabilities
- **Wireless Communication**: Supports Wi-Fi, GSM (SIM7000G), and LoRa P2P
- **Sensor Interfaces**: Digital Input/Output, Analog Input, Modbus RTU
- **Real-Time Cloud Transmission**: Sends data via HTTP POST to Favoriot
- **Local Data Logging**: Backup via SD card in CSV format
- **Configurable System**: Reads setup from SD card (tool by IT partner)
- **Power-Protected Design**: Includes TVS, zener diodes, and relay-based sensor control

---

## 🔧 Technologies Used

**Microcontrollers:**
- ESP32 (main control and communication)
- Arduino Pro Mini (expansion node)

**Communication Modules:**
- SIM7000G (GSM LTE)
- RA-02 LoRa Module

**Peripheral Modules:**
- SD Card Module
- RTC Module (DS1307)
- GPIO Expander (MCP23017)
- ADC (ADS1115)
- MAX485 (Modbus RTU interface)

**Protocols:**
- HTTP POST (Wi-Fi/GSM)
- LoRa P2P
- Modbus RTU

---

## 🗂️ Folder Structure

📁 Firmware → PlatformIO/Arduino firmware code
📁 Hardware → Schematics, PCB layout, BOM
📁 Documentation → Test plans, control narratives, system diagrams
📁 Tools → SD card config tool, scripts


---

## 📷 Media (Coming Soon)

- System architecture block diagram  
- Hardware photos  
- Dashboard screenshot (Favoriot)  

---

## 🚧 Challenges & Solutions

| Challenge                         | Solution                                                   |
|----------------------------------|-------------------------------------------------------------|
| Flash memory limitation (Arduino)| Switched to ESP32 for more complex data processing         |
| Sensor power consumption         | Added relay to switch sensors only during acquisition       |
| GSM/LoRa interference            | Used transient suppressors and improved antenna isolation   |
| Cloud connection dropouts        | Used SD card buffering and auto-sync after reconnect        |

---

## 📈 Impact

- Enabled real-time fig farm irrigation and monitoring  
- Reduced manual effort in industrial data collection  
- Modular setup allows easy customization and scaling  

---

## 👨‍💻 Author

**Ts. Muhammad Nazur Syahmi Bin Mohd Nasir**  
📧 nazur.syahmi@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/nazursyahmi/) | [GitHub](https://github.com/nazur030)

---

## 📅 Project Status

✅ Alpha-tested  
🛠️ Preparing for field deployment  
📤 Ready for portfolio showcase
