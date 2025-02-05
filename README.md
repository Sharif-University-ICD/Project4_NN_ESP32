# **ICD Project: SoC Estimation using ESP32 and Neural Networks**  

## **Overview**  
This project focuses on **State-of-Charge (SoC) estimation for Li-Ion batteries** using **Deep Neural Networks (DNNs)** on an **ESP32 board**. The neural network predicts the SoC based on **current, voltage, and temperature data**, and the results are transmitted through various communication protocols.  

## **Project Steps**  
### **1. Neural Network Implementation**  
- Based on the paper *"State-of-Charge Estimation of Li-Ion Battery in Electric Vehicles: A Deep Neural Network Approach"*.  
- Training performed using TensorFlow and converted to **TensorFlow Lite** for ESP32 deployment.  

### **2. ESP32 Deployment**  
- The trained model is implemented on ESP32 using **TensorFlowLite_ESP32**.  
- The inference engine is written in C++ for execution on the ESP32.  

### **3. Communication Protocols**  
Implemented for data transmission between ESP32 and other devices:  
- **UART (Serial)**  
- **Wi-Fi**  
- **Bluetooth Low Energy (BLE)**  

### **4. Performance Evaluation**  
- Comparison of **inference time** and **data transmission speed** for different protocols.  

## **Results**  
- **UART** was the fastest but required wired connections.  
- **Wi-Fi and BLE** were comparable in performance, with **BLE being more power-efficient**.  

## **Conclusion**  
The choice of communication protocol depends on the application. **UART** is suitable for fast, wired connections, while **BLE/Wi-Fi** are better for IoT applications.  

---

📌 **Contributors**  
- **Farzam Koohi-Ronaghi**  
- **Sana Babayan Vanestan**  
