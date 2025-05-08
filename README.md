# Driftel 🛰️🚁  
**Smart Delivery Drone with Real-Time IoT Tracking**

Driftel is an open-source project to simulate or build a lightweight delivery drone capable of navigating to predefined GPS coordinates and updating its position in real-time using IoT technologies. It combines drone flight control with live tracking, user notifications, and safety-first design.

## 🔧 Features

- 📦 Autonomous delivery of lightweight packages
- 🌍 GPS-based predefined waypoint navigation
- 📡 Real-time location tracking using IoT (MQTT/HTTP/WebSocket)
- 📲 User mobile notification integration (via Telegram, WhatsApp, or SMS)
- 🧠 Simulation mode available for testing without hardware
- 🔋 Battery and altitude monitoring
- 🛡️ Built-in safety and fail-safe measures

## 📡 Tech Stack

- **Hardware (Optional):** Arduino / ESP32 + GPS module + Drone frame
- **IoT Communication:** MQTT (via Mosquitto) or HTTP REST API
- **Frontend (Optional):** React or Svelte web dashboard for tracking
- **Mobile Alerts:** IFTTT, Telegram Bot API, or Twilio
- **Backend (Optional):** Node.js or Python Flask/FastAPI for message routing
- **Simulation:** Python or Unity for simulating flight paths

## 🗺️ Use Case

1. User sets delivery coordinates.
2. Drone lifts off and flies to the target location.
3. Real-time position updates are sent to the backend.
4. User receives notifications during key stages (takeoff, en-route, delivery).
5. Drone returns or lands safely.

## 🛑 Safety Considerations

- **No-Fly Zone Awareness:** Avoids airports and restricted areas using built-in zone maps.
- **Failsafe Return:** Returns to home if GPS signal is lost or battery is low.
- **Weather Caution:** Not designed for use in rain or high winds.
- **Weight Limit:** Only lightweight objects under 500g.
- **Legal Compliance:** Always check local UAV laws and flight restrictions before using outdoors.

## 📁 Folder Structure

```

/Driftel
├── firmware/        # ESP32 or Arduino code
├── simulator/       # Flight simulator (Python/Unity)
├── backend/         # API and message broker integration
├── dashboard/       # Web UI to track drone
├── docs/            # Technical documentation
└── mobile/          # Mobile integration (bot/API)

````

## 🛠️ Getting Started

1. Clone the repo:
```bash
   git clone https://github.com/sosyalrobot/Driftel.git
   cd Driftel
````

2. Choose **simulator** or connect real **ESP32 + GPS module**.
3. Run backend server:

   ```bash
   cd backend
   npm install
   npm start
   ```
4. Launch dashboard to monitor drone in real-time.

## 📄 License

MIT License. Free to modify and distribute.

---

**Driftel** – bringing smart air delivery to your fingertips.
