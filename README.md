# 🎤 VoiceNest – Voice Controlled Home Automation using VC02

## 📌 Project Overview
VoiceNest is a voice-controlled home automation system built using the VC02 voice recognition module. The system allows users to control electrical appliances such as lights and fans using simple voice commands without requiring internet connectivity or a microcontroller.

---

## 🎯 Objectives
- To develop a voice-controlled automation system
- To eliminate the need for manual switches
- To create an offline and low-cost smart home solution

---

## ⚙️ Features
- 🎙️ Voice-controlled appliance operation
- 🌐 Works completely offline (no internet required)
- 💡 Multiple device control (LEDs / lights / fan)
- ⚡ Direct GPIO control (no Arduino required)
- 🔋 Power saving using wake-up and sleep commands
- 🔊 Audio response using speaker

---

## 🧠 System Working
Voice Command → VC02 Module → GPIO Output → Relay/LED → Appliance Control

---

## 🔌 Hardware Components
- VC02 Voice Recognition Module  
- Microphone  
- Speaker  
- Relay Module (or LEDs for testing)  
- HLK-PM01 AC-DC Power Module  
- Breadboard & Connecting Wires  

---

## 🔧 Software & Tools
- VC02 Voice SDK (Ai-Thinker Platform)  
- GitHub (for documentation)  
- YouTube (for reference learning)  

---

## 🔌 Circuit Connections
- VC02 VCC → 5V Power Supply  
- VC02 GND → Ground  
- GPIO Pins → Relay Inputs / LEDs  
- Microphone → Voice Input  
- Speaker → Audio Output  

---

## 💡 Example Command Mapping
| Voice Command | GPIO | Action |
|--------------|------|--------|
| Light ON | GPIO_B0 | HIGH |
| Light OFF | GPIO_B0 | LOW |
| Second Light ON | GPIO_B1 | HIGH |
| Second Light OFF | GPIO_B1 | LOW |
| Fan ON | GPIO_B7 | HIGH |

---

## 🔋 Power Management
- Wake-up command activates system
- Sleep command reduces power consumption
- Improves efficiency and avoids unnecessary processing

---
