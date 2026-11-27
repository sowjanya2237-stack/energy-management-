# AI-Driven Smart Energy Management for Polar Research Stations

## About the Project

AI-Driven Smart Energy Management for Polar Research Stations is an intelligent energy monitoring and optimization system designed to improve energy utilization in polar research environments.

The project integrates IoT sensors, machine learning, optimization techniques and a web-based dashboard to monitor electrical energy consumption and environmental conditions.

The system uses an ESP32 to collect sensor data, a FastAPI backend to process and manage the data, PostgreSQL for database storage, and a React dashboard to display monitoring results. XGBoost is used for energy demand prediction, while OR-Tools supports energy resource optimization.

## Features

- **Real-Time Energy Monitoring:** Monitors electrical parameters such as voltage, current, power and energy consumption.
- **Environmental Monitoring:** Collects temperature, humidity and light intensity using connected sensors.
- **IoT Integration:** Uses ESP32 to collect sensor readings and communicate with the backend.
- **AI-Based Energy Prediction:** Uses the XGBoost machine learning algorithm to predict energy demand.
- **Energy Optimization:** Uses Google OR-Tools to support efficient energy resource allocation.
- **Interactive Dashboard:** Displays energy and environmental information through a React-based dashboard.
- **Alerts and Monitoring:** Helps identify unusual energy consumption patterns.
- **Data Visualization:** Presents energy trends, predictions and monitoring information through graphical reports.
- **Renewable Energy Management:** Supports monitoring and management of renewable energy resources.

## Technologies Used

### Frontend
- React.js
- JavaScript
- HTML
- CSS

### Backend
- Python
- FastAPI
- SQLAlchemy

### Database
- PostgreSQL

### AI and Optimization
- XGBoost
- Google OR-Tools

### IoT and Hardware
- ESP32
- DS18B20 Temperature Sensor
- DHT22 Temperature and Humidity Sensor
- BH1750 Light Sensor
- PZEM-004T Energy Meter

### Development Tools
- Visual Studio Code
- Arduino IDE
- Git
- GitHub

## System Architecture

The system follows a layered architecture:

1. **Sensor Layer:** Collects electrical and environmental data using connected sensors.
2. **Controller Layer:** ESP32 reads sensor values and sends the data to the backend.
3. **Backend Layer:** FastAPI handles data processing and application operations.
4. **Database Layer:** PostgreSQL stores the required monitoring information.
5. **AI and Optimization Layer:** XGBoost performs energy demand prediction, and OR-Tools supports energy optimization.
6. **Frontend Layer:** React displays the information through an interactive dashboard.

## Project Structure

```text
energy-management-/
│
├── ARDUINO SENSOR CODE/
│
├── backend/
│   ├── app/
│   ├── requirements.txt
│   └── ...
│
├── frontend/
│   ├── src/
│   ├── package.json
│   └── ...
│
└── .gitignore
```

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/sowjanya2237-stack/energy-management-.git
cd energy-management-
```

### 2. Backend Setup

Open a terminal and navigate to the backend folder.

```bash
cd backend
```

Install the required Python packages.

```bash
pip install -r requirements.txt
```

Configure the PostgreSQL database connection using the backend environment configuration.

Start the FastAPI server:

```bash
uvicorn app.main:app --host 0.0.0.0 --port 8000 --reload
```

The backend API documentation can be accessed at:

```text
http://localhost:8000/docs
```

### 3. Frontend Setup

Open another terminal and navigate to the frontend folder.

```bash
cd frontend
```

Install the dependencies:

```bash
npm install
```

Start the React development server:

```bash
npm run dev
```

Open the local URL displayed in the terminal to access the dashboard.

### 4. ESP32 Setup

1. Open the Arduino sensor code using Arduino IDE.
2. Select the appropriate ESP32 board.
3. Configure the Wi-Fi credentials.
4. Configure the backend server address.
5. Connect the required sensors to the configured GPIO pins.
6. Upload the program to the ESP32.
7. Verify sensor readings and data communication with the backend.

## Project Outcome

The completed system combines IoT-based monitoring, AI-driven energy demand prediction and optimization techniques in a unified energy management application.

It provides a centralized dashboard for monitoring energy consumption and environmental conditions while supporting efficient energy utilization in polar research stations.

