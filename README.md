# Weather App (MQTT + SQLite)

## Overview
The **Weather App** collects temperature and humidity data via **MQTT**, stores it in **SQLite**, and displays it on a web interface using **Chart.js**.

---

## Features
✅ Real-time weather data collection  
✅ MQTT-based communication  
✅ SQLite database storage  
✅ REST API for data retrieval  
✅ Web visualization with Chart.js  

---

## Setup Instructions
### **1️⃣ Install Dependencies**
```sh
npm install express sqlite3 mqtt cors

### **2️⃣ Run the Server
sh
Copy
Edit
node server.js

### **3️⃣ Open Web Interface
Simply open index.html in a browser.

MQTT Configuration
Broker: ws://157.173.101.159:9001
Subscribed Topics:
/work_group_01/room_temp/temperature
/work_group_01/room_temp/humidity

Database Schema
sql
Copy
Edit
CREATE TABLE IF NOT EXISTS sensor_data (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    topic TEXT,
    value TEXT,
    timestamp DATETIME DEFAULT CURRENT_TIMESTAMP
);

 Author
UWAYO Ange Kevine
🔗 GitHub: Angek12
📧 Email: angeekevinee@gmail

