# AR Air Quality Monitor 🌬️

An interactive web-based Augmented Reality application for real-time air quality visualization and environmental education. This system transforms abstract air pollution data into immersive, understandable visual experiences using AR.js technology.

## 🎯 Overview

The AR Air Quality Monitor is an advanced IoT-based system that combines hardware sensors with cutting-edge AR visualization to provide real-time air quality monitoring. The system uses marker-based AR to display environmental data in an interactive 3D format, making air pollution education more engaging and effective.

## ✨ Key Features

- **Real-time Air Quality Monitoring**: Live PM1.0, PM2.5, and PM10 particle measurement
- **Interactive AR Visualization**: 5 different AR display screens based on air quality levels
- **Color-coded Classification**: Visual indicators from "So Good" (Green) to "Hazardous" (Purple)
- **Web-based AR**: No app installation required - runs directly in web browsers
- **Firebase Integration**: Real-time database synchronization for instant data updates
- **Educational Focus**: Designed to improve environmental awareness and understanding

## 🛠️ System Architecture

### Hardware Components
- **ESP32 Microcontroller**: Main processing unit for data collection and wireless communication
- **PMS5003 Particle Sensor**: High-precision sensor for detecting PM1.0, PM2.5, and PM10 particles
- **OLED Display**: Local display for real-time sensor readings

### Software Stack
- **AR.js**: Web-based augmented reality framework
- **Firebase Realtime Database**: Cloud backend for data storage and synchronization
- **Arduino IDE**: Programming environment for ESP32
- **HTML5/CSS3/JavaScript**: Frontend web technologies

## 📊 Air Quality Classification

| PM2.5 Range (μg/m³) | Status | Color | Health Impact |
|---------------------|--------|-------|---------------|
| 0 - 30 | So Good | 🟢 Green | Minimal health impact |
| 31 - 60 | Healthy | 🔵 Light Blue | Minimal health impact |
| 61 - 90 | Normal | 🟡 Yellow | Acceptable for sensitive groups |
| 91 - 130 | Very Unhealthy | 🟠 Orange | Health warning for all |
| ≥130 | Hazardous | 🟣 Purple | Emergency conditions |


## 📱 Usage

### Accessing the AR Application
1. Navigate to the deployed web application
2. Allow camera permissions when prompted
3. Point your device camera at the Hiro marker
4. The AR visualization will appear showing real-time air quality data

### AR Marker
The system uses the standard Hiro marker for AR tracking. You can:
- Print the marker from the repository
- Display it on another screen
- Use any Hiro marker available online

### Real-time Data Flow
1. **Sensor Reading**: ESP32 reads data from PMS5003 every second
2. **Local Display**: Data shown on OLED screen
3. **Cloud Sync**: Data sent to Firebase Realtime Database
4. **AR Update**: Web application receives updates and refreshes AR display

## 🎨 AR Display Features

Each air quality level provides a unique AR experience:
- **Dynamic Color Coding**: Background colors change based on air quality
- **Real-time Values**: Live numerical data for all particle sizes
- **Health Information**: Contextual health warnings and recommendations
![Screenshot 2025-05-30 161048](https://github.com/user-attachments/assets/affd01c2-8298-4a66-8032-18fd36747b8e)
![Screenshot 2025-05-30 161007](https://github.com/user-attachments/assets/1f612948-21ba-47c3-b9b4-53e56d93813d)
![Screenshot 2025-05-30 161609](https://github.com/user-attachments/assets/bc04a516-971d-411d-9141-d3f1644360d6)
![Screenshot 2025-05-30 161835](https://github.com/user-attachments/assets/c94eb195-0627-48b5-aa50-67fd9de72f67)
![Screenshot 2025-05-30 161955](https://github.com/user-attachments/assets/05d50d41-888e-4c5b-9a11-7fe384af6081)


## 📈 Research & Validation

This system has been validated through academic research involving 31 student respondents:
- **96.8%** considered air quality education important
- **87.1%** believed AR helps understand complex environmental topics
- **93.5%** showed interest in AR-based educational applications

## 🔗 Links

- **Live Demo**: [https://brand750.github.io/ar-air-quality-monitor/](https://brand750.github.io/ar-air-quality-monitor/)

## 🙏 Acknowledgments

- AR.js community for the amazing web AR framework
- Firebase team for reliable real-time database services
- Environmental education researchers for inspiration and validation
- All survey participants who helped validate the system effectiveness
