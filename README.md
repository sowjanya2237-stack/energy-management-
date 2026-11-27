# IoT-Based Smart Energy Monitoring and Optimization System

### AI-Based Smart Energy Management for Polar Research Stations

## About the Project

This project focuses on developing an intelligent energy monitoring and optimization system for polar research stations.

It combines IoT sensors, machine learning and a web-based dashboard to monitor electrical energy consumption and environmental conditions. The system aims to support efficient energy usage and better energy management.

## Features

- **Real-Time Energy Monitoring:** Monitor electrical parameters such as voltage, current and power.
- **Environmental Monitoring:** Collect temperature, humidity and light intensity data using sensors.
- **IoT Integration:** Use ESP32 to collect sensor readings and communicate with the backend.
- **Web Dashboard:** Display energy and environmental data through an interactive interface.
- **Energy Prediction:** Explore machine learning-based energy consumption prediction.
- **Energy Optimization:** Work towards improving energy utilization using optimization techniques.
- **Monitoring and Alerts:** Support identification of unusual energy consumption patterns.

## Technologies Used

### Frontend
- React
- JavaScript

### Backend
- Python
- FastAPI
- SQLAlchemy

### Database
- PostgreSQL

### Machine Learning and Optimization
- XGBoost
- OR-Tools

### Hardware and Sensors
- ESP32
- DS18B20 Temperature Sensor
- DHT22 Temperature and Humidity Sensor
- BH1750 Light Sensor
- PZEM-004T Energy Monitoring Module

## System Architecture

1. **Sensor Layer:** Sensors collect electrical and environmental readings.
2. **Controller Layer:** ESP32 reads sensor values and sends data to the backend.
3. **Backend Layer:** FastAPI handles incoming data and application requests.
4. **Database Layer:** PostgreSQL stores monitoring information.
5. **Frontend Layer:** React displays the collected data through dashboards.
6. **Prediction and Optimization:** Machine learning and optimization techniques support energy management.

## Project Structure

```text
energy-management-/
|
|-- backend/
|   |-- FastAPI application
|   |-- Database and API modules
|
|-- frontend/
|   |-- React application
|
|-- ARDUINO SENSOR CODE/
|   |-- ESP32 sensor programs
|
|-- .gitignore
```

## Installation and Setup

### Prerequisites
- Python
- Node.js and npm
- PostgreSQL
- Git
- Arduino IDE (for ESP32 sensor integration)

### 1. Clone the Repository

```bash
git clone https://github.com/sowjanya2237-stack/energy-management-.git
```

### 2. Backend Setup

```bash
cd backend
pip install -r requirements.txt
```

Configure the PostgreSQL database connection in the backend `.env` file.

Start the backend:

```bash
uvicorn app.main:app --host 0.0.0.0 --port 8000 --reload
```

### 3. Frontend Setup

Open another terminal:

```bash
cd frontend
npm install
npm run dev
```

### 4. ESP32 Setup

- Open the sensor program in Arduino IDE.
- Select the appropriate ESP32 board and COM port.
- Configure the Wi-Fi and backend connection details.
- Upload the program to the ESP32.

## Project Goal

To develop an intelligent energy management solution that helps monitor energy consumption, improve energy efficiency and support reliable energy utilization in polar research environments.

## Author

Sowjanya P.

GitHub: https://github.com/sowjanya2237-stack
