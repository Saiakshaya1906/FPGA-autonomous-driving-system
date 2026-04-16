# 🚗 FPGA-Based Autonomous Driving System

## 📌 Overview

This project presents a **Supervised Learning-Based Autonomous Driving System** integrated with **FPGA for real-time output display**.

A simulation environment is created using PyGame, where driving data is collected, processed, and used to train a machine learning model. The predicted steering decisions are transmitted to an FPGA board and displayed using hardware.

---

## 🧠 System Architecture

Simulation → Image Processing → ML Model → Prediction → Serial Communication → FPGA → Display

---

## 🎯 Project Title

**Supervised Learning-Based Autonomous Driving System with FPGA-Based Real-Time Output**

---

## ⚙️ Technologies Used

* Python
* OpenCV
* PyGame
* NumPy
* Serial Communication (PySerial)
* FPGA (Basys 3)
* Verilog HDL
* Xilinx Vivado

---

## 📁 Project Structure

```
python_codes/   → Simulation, ML model, communication  
verilog/        → FPGA design (UART + display)  
dataset/        → Sample training images  
results/        → Output results  
```

---

## 🚀 Features

* Simulation-based autonomous driving
* Dataset collection and labeling
* Image preprocessing using OpenCV
* Real-time steering prediction
* PC ↔ FPGA communication
* FPGA-based output display
* Lightweight ML implementation

---

## ▶️ How to Run

### 1️⃣ Collect Dataset

```bash
python python_codes/manual_simulator.py
```

### 2️⃣ Train Model

```bash
python python_codes/train_csv.py
```

### 3️⃣ Extract Weights

```bash
python python_codes/extract_weights.py
```

### 4️⃣ Run Autonomous Simulation

```bash
python python_codes/autonomous_simulator.py
```

### 5️⃣ Run FPGA Interface

```bash
python python_codes/pygame_fpga.py
```

---

## 📦 Requirements

Install required libraries:

```bash
pip install pygame numpy opencv-python pyserial
```

### FPGA Requirements

* Xilinx Vivado
* Basys 3 FPGA Board
* Proper USB drivers

---

## 🖥️ Hardware Used

* Basys 3 FPGA Board
* USB Interface
* Computer System

The FPGA receives steering commands from the PC and displays them using a 7-segment display.

---

## 📊 Dataset Note

The dataset is generated using manual driving in the simulation. Only sample images are included due to size limitations.

---

## 🔮 Future Improvements

* CNN-based deep learning model
* Real-time camera input
* Embedded system integration
* Advanced FPGA visualization

---

## 👨‍💻 Author

Sai Akshaya
