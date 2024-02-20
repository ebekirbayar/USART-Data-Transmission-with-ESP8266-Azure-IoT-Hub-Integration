<br/>
<p align="center">
  <a href="https://github.com/ebekirbayar/USART-Data-Transmission-with-ESP8266-Azure-IoT-Hub-Integration">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">USART Data Transmission with ESP8266: Azure IoT Hub Integration</h3>

  <p align="center">
    In this project, we explore the integration of ESP8266 with Azure IoT Hub through USART communication. The ESP8266 microcontroller is utilized to transmit data received over USART to the Azure IoT Hub platform. This integration enables seamless communication between the ESP8266 device and Azure's cloud infrastructure, facilitating efficient data transfer and analysis for IoT applications.
    <br/>
    <br/>
    <a href="https://github.com/ebekirbayar/USART-Data-Transmission-with-ESP8266-Azure-IoT-Hub-Integration">View Demo</a>
    .
    <a href="https://github.com/ebekirbayar/USART-Data-Transmission-with-ESP8266-Azure-IoT-Hub-Integration/issues">Report Bug</a>
    .
    <a href="https://github.com/ebekirbayar/USART-Data-Transmission-with-ESP8266-Azure-IoT-Hub-Integration/issues">Request Feature</a>
  </p>
</p>
<p align="center">

![Contributors](https://img.shields.io/github/contributors/ebekirbayar/USART-Data-Transmission-with-ESP8266-Azure-IoT-Hub-Integration?color=dark-green) ![Issues](https://img.shields.io/github/issues/ebekirbayar/USART-Data-Transmission-with-ESP8266-Azure-IoT-Hub-Integration) ![License](https://img.shields.io/github/license/ebekirbayar/USART-Data-Transmission-with-ESP8266-Azure-IoT-Hub-Integration) 

</p>
## Table Of Contents

* [About the Project](#about-the-project)
* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)
* [Usage](#usage)
* [Roadmap](#roadmap)
* [License](#license)
* [Authors](#authors)

## About The Project
<p align="center">
 <img src="images/screenshot.jpeg" alt="Screenshot" width="400" height="auto">
</p>

# Detailed Project Description

## Overview

This project utilizes an ESP8266 microcontroller along with a USART communication module to collect data and send it to Azure IoT Hub for further processing and analysis. The ESP8266 acts as the main controller, collecting data from the USART interface and establishing a connection with the Azure IoT Hub using the MQTT protocol for data transmission.

## Requirements

- Arduino IDE

## Project Components
- ESP8266 Microcontroller

The ESP8266 microcontroller serves as the central processing unit in this project. It is responsible for interfacing with the USART communication module, establishing a WiFi connection, and sending data to the Azure IoT Hub.

## USART Communication Module

- The USART communication module is used to interface with external devices or sensors that communicate via USART protocol. It facilitates the transfer of data between the ESP8266 microcontroller and external devices.

## Azure IoT Hub
- Azure IoT Hub is a managed service provided by Microsoft Azure for securely connecting, monitoring, and managing IoT devices. In this project, Azure IoT Hub serves as the central hub for receiving and processing data from the ESP8266 microcontroller.

## Project Workflow
- Data Acquisition: The ESP8266 microcontroller reads data from external devices or sensors via the USART communication module.

- Data Processing: The collected data may undergo preprocessing or filtering as required by the application logic.

- Azure IoT Hub Connection Establishment: The ESP8266 establishes a secure connection with the Azure IoT Hub using the MQTT protocol.

- Data Transmission: Once connected, the ESP8266 sends the processed data to the Azure IoT Hub at regular intervals.

- Data Analysis and Visualization: Data received by the Azure IoT Hub can be further analyzed, visualized, and acted upon using Azure services such as Azure Stream Analytics, Azure Functions, or Azure Web Apps.

## Benefits and Applications

- Real-time Monitoring: The project enables real-time monitoring of data, allowing for immediate response to changes or anomalies.

- Remote Data Collection: By leveraging Azure IoT Hub, data can be collected from multiple ESP8266 devices deployed in different locations, enabling centralized data management and analysis.

- Predictive Maintenance: Data collected through USART communication can be used to monitor the condition

## Getting Started


### Prerequisites

- Arduino IDE
- ESP8266WiFi library
- PubSubClient library
- ArduinoJson library
- Azure IoT C SDK
- Azure IoT Hub account and device registration
- WiFi network credentials

### Installation

1.	Arduino IDE Setup: Download and install Arduino IDE from the official website.

2.	Library Installation: Open Arduino IDE and install the required libraries using Sketch > Include Library > Manage Libraries:
      •	ESP8266WiFi
      •	PubSubClient
      •	ArduinoJson

```sh
git clone https://github.com/ebekirbayar/USART-Data-Transmission-with-ESP8266-Azure-IoT-Hub-Integration.git
```

3.	Azure IoT C SDK Setup: We are using a custom version of the Azure IoT C SDK for Arduino. Download the Arduino SDK.

4.	WiFi Configuration: Update WiFi network credentials (IOT_CONFIG_WIFI_SSID and IOT_CONFIG_WIFI_PASSWORD) and Azure IoT Hub settings (IOT_CONFIG_IOTHUB_FQDN, IOT_CONFIG_DEVICE_ID, IOT_CONFIG_DEVICE_KEY) in the iot_configs.h file.

```JS
   // Wifi
     #define IOT_CONFIG_WIFI_SSID "YOUR WIFI SSID"
     #define IOT_CONFIG_WIFI_PASSWORD "your_password"

   // Azure IoT
     #define IOT_CONFIG_IOTHUB_FQDN "xxxxxxxxxxx"
     #define IOT_CONFIG_DEVICE_ID "Your_Device_ID"
     #define IOT_CONFIG_DEVICE_KEY "Your_Device_Key_xxxxxxxxxxxxxxxxxxxx"
```

5.	Uploading Code: Upload the code in Arduino IDE and flash it to your ESP8266 device.

## Usage

Usage
    
    •	Power up the device and open the serial monitor.
    •	The ultrasonic sensor measures distance, and the data is sent to Azure IoT Hub.
    •	You can view the data in the Azure IoT Hub console.

## Roadmap

1.  Setting Up Arduino IDE:
• Download and install the Arduino IDE from the official website.
• Open Arduino IDE and install the necessary libraries via Sketch > Include Library > Manage Libraries.

2. Installing Libraries:
• Install the ESP8266WiFi, PubSubClient libraries using the Library Manager in Arduino IDE.

3. Configuring Azure IoT SDK:
• Download the custom Azure IoT C SDK for Arduino from the provided link.
• Follow the instructions in the SDK documentation to set it up in your Arduino IDE.

4. Updating WiFi and Azure IoT Hub Credentials:
• Open the iot_configs.h file and update the WiFi SSID, password, IoT Hub FQDN, device ID, and device key.

5. Uploading the Code:
• Compile and upload the code to your ESP8266 device via Arduino IDE.

6. Running the Project:
• Power on the device and open the serial monitor in Arduino IDE.
• Observe the data being sent to Azure IoT Hub.

## License

Distributed under the MIT License. See [LICENSE](https://github.com/ebekirbayar/USART-Data-Transmission-with-ESP8266-Azure-IoT-Hub-Integration/blob/main/LICENSE) for more information.

## Authors

* **Ebubekir BAYAR** - *Computer Engineer* - [Ebubekir BAYAR](https://github.com/ebekirbayar/)