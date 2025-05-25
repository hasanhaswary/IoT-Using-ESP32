# 🌐 IoT Integrated Solution

**Platform** | **License** | **Status** | **Hardware**\
ESP32 | MIT License | In Development | ESP32 Boards x5

---

## 📖 Overview

A robust IoT Integrated Solution designed to monitor environmental parameters like temperature, humidity, and light intensity using ESP32 boards. This project features multiple sender nodes that collect data and transmit it wirelessly to a receiver node, which displays the information on a user-friendly dashboard. Perfect for real-time environmental monitoring with a cyberpunk-inspired setup!

---

## IMPLEMENTATION DIAGRAM
![Final IOT Solution Diagram](https://github.com/user-attachments/assets/7efce2a9-8a80-4eec-a2a6-a30af7ef20b6)

---

## ✨ Features

- 📡 Wireless P2P communication (5-second intervals) for seamless data transfer
- 🌡️ Four sender nodes collecting:
  - **Node 1 (ID:1)**: Temperature, humidity, and light
  - **Node 2 (ID:2)**: Temperature, humidity, and light
  - **Node 3 (ID:3)**: Temperature
  - **Node 4 (ID:4)**: Humidity and light
- 📊 Receiver node with a UI dashboard displaying real-time data
- 🖥️ UI Dashboard with sections for:
  - Temperature, humidity, and light readings per node
  - Visual feedback for each node’s data
- 🔄 Efficient data transmission using ESP32 boards
- ⚙️ Scalable system for adding more nodes

---

## 🎮 Controls

- **Sender Nodes**: Automatically collect and send data every 5 seconds via wireless P2P communication
- **Receiver Node**: Displays data on the UI dashboard with no manual interaction required

### UI Screenshots

![Screenshot 2025-05-25 202010](https://github.com/user-attachments/assets/1deae4e3-aada-4da9-955e-438ac5c6a8de)

---

## 🛠️ Technical Details

Built with ESP32 boards, this project features:

- Wireless P2P communication for data transfer
- Structured data packets: `int id`, `float temperature`, `float humidity`, `int light`, `int readingId`
- UI dashboard for real-time visualisation of environmental data
- Modular node architecture for easy scalability
- Efficient power management for continuous operation

---

## 🚀 Getting Started

### Installation (For Users)

1. **Set Up Hardware**:
   - Connect the ESP32 boards as shown in the system diagram.
   - Ensure all boards are powered and configured for wireless P2P communication.
2. **Upload Firmware**:
   - Download the firmware from the Releases page.
   - Flash the firmware onto each ESP32 board using an appropriate tool (e.g., ESP32 Flash Download Tool).
3. **Launch the System**:
   - Power on all ESP32 boards.
   - Access the UI dashboard on the receiver node to view real-time data.

### Installation (For Developers/Contributors)

1. **Fork the Repository**: Fork this repository to your GitHub account.
2. **Clone the Repository**:
   - Clone the repository:

     ```
     git clone <your-forked-repo-url>
     ```
3. **Set Up Development Environment**:
   - Open the project in your preferred IDE (e.g., Arduino IDE or PlatformIO).
   - Ensure the ESP32 board support package is installed.
4. **Upload and Test**:
   - Upload the code to each ESP32 board.
   - Test the system by monitoring the receiver node’s UI dashboard data.

---

## 🎯 How to Use

1. Power on all ESP32 boards (sender and receiver nodes).
2. Sender nodes will automatically collect data (temperature, humidity, light) every 5 seconds.
3. The receiver node will display the data on the UI dashboard, categorised by node ID.
4. Monitor the dashboard for real-time environmental updates.

---

## 💡 Development Notes

### Architecture

The system is structured around these key components:

- **Sender Nodes (ID:1-4)**: Collect environmental data and transmit it wirelessly.
- **Receiver Node**: Receives data and updates the UI dashboard.
- **Wireless P2P Communication**: Ensures efficient data transfer between nodes.
- **UI Dashboard**: Displays data in an organised format for each node.

### Known Issues

- Occasional data packet loss during high-interference environments.
- UI dashboard refresh rate may lag with a high number of nodes.

---

## 📝 Future Enhancements

- Add data logging to store historical readings.
- Implement alerts for abnormal environmental conditions.
- Enhance the UI dashboard with graphical data visualisation (e.g., charts).
- Optimise power consumption for sender nodes.
- Support additional sensors for more data types (e.g., air quality).

---

## 🤝 Contributions

We welcome contributions to enhance the IoT Integrated Solution! To contribute:

1. **Fork the Repository**: Fork this repo to your GitHub account.
2. **Make Changes**: Create a new branch for your feature or bugfix (`git checkout -b feature/your-feature-name`).
3. **Commit and Push**: Commit your changes and push to your fork (`git push origin feature/your-feature-name`).
4. **Submit a Pull Request**: Open a pull request against the main branch of this repository, describing your changes in detail.

---

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

## 👏 Acknowledgments

- Inspired by IoT monitoring systems and wireless communication projects.
- Thanks to the ESP32 community for resources and support.

---

## 📚 Citations/References

- Espressif Systems provide ESP32 documentation and libraries.
- Wireless P2P communication protocols inspired by open-source IoT projects.
