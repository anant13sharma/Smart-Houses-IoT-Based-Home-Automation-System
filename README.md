
# Important Note 

- The complete project documentation, including objectives, hardware/software details, wiring, setup, and circuit explanations, is available in the uploaded project report (PDF) in this repository. I have not created a separate file specifically for the code, as everything has been documented thoroughly in the report.
  Apologies for the inconvenience — but the report should be more than sufficient to understand and replicate the entire project. Thank you for your understanding.


# Overview

- This project aims to build a smart home automation system using open-source microcontrollers and cloud-based tools. It allows users to control electrical appliances like lights and fans through mobile apps, voice commands (via Google Assistant), and automation services like IFTTT. 
-The system is designed using Arduino, NodeMCU (ESP8266), Blynk App, and Webhooks, and demonstrates how microcontrollers can be connected to the internet to enable real-time interaction with physical devices.
- Note: A detailed PDF project report is included in this repository for reference.

# Objective

- The goal is to create a system that integrates with household appliances and bridges them to the internet using Wi-Fi and programmable controllers. It simplifies daily tasks, adds convenience, and introduces automation at a minimal cost.

# Hardware Used

- Arduino UNO / Mega
- NodeMCU (ESP8266 Wi-Fi module)
- Relay Modules (2-channel and 4-channel)
- Arduino Ethernet Shield
- Jumper Wires
- Breadboard
- Bulb and Holder
- 12V DC Adapter
- AC 220V Power Supply

# Software & Platforms

- Arduino IDE (for firmware development)
- Blynk App (for remote control via phone)
- IFTTT (to connect Google Assistant with Blynk)
- Webhooks (to handle HTTP requests from IFTTT)
- Google Assistant (for voice control)

# How It Works

- Manual Control using Blynk:
- A project is created in the Blynk app.
- Buttons are configured to control pins on NodeMCU.
- When a button is pressed in the app, it sends commands to NodeMCU via the Blynk Cloud.
- Voice Control using Google Assistant and IFTTT:
- Google Assistant is configured to trigger IFTTT applets.
- IFTTT uses Webhooks to send HTTP requests to the Blynk server.
- The requests update specific digital pins on NodeMCU to control appliances.
- NodeMCU acts as a bridge between the internet and connected devices, interpreting commands and toggling relays accordingly.

# Setup Guide

- Install Arduino IDE and necessary ESP8266 board definitions.
- Clone or download the code from:
- GitHub Repository
- Configure the .ino file with:
- Blynk Auth Token
- Wi-Fi SSID and Password
- Upload the sketch to NodeMCU using Arduino IDE.
- Set up Blynk project and buttons in the mobile app.
- Create IFTTT Applets to connect voice commands to Blynk Webhook URLs.
- Wire the NodeMCU and Relay module as per the README instructions in the GitHub repo.

# Features

- Remote control of appliances using mobile app
- Voice control through Google Assistant
- Event automation using IFTTT and Webhooks
- Real-time relay control via internet
- Scalable to multiple devices (up to 32 relays)

# Future Scope

- Add IR control for ACs, TVs using Arduino Mega
- Monitor distances using ultrasonic sensors
- Expand to include sensors and device feedback
- Automate more complex workflows using additional APIs
