# 🔋 Battery Management System (BMS) Simulation

## 📌 Project Overview

This project is a simplified Battery Management System (BMS) simulation developed using Python.

The simulation monitors important battery parameters such as:

- State of Charge (SOC)
- State of Health (SOH)
- Battery voltage
- Battery temperature
- Heat generation
- Charging and discharging behavior
- Basic battery safety conditions

The project demonstrates how a BMS can monitor battery conditions and identify abnormal operating conditions.

---

## 🎯 Objectives

The main objectives of this project are:

1. Simulate battery charging and discharging.
2. Calculate the State of Charge (SOC).
3. Estimate the State of Health (SOH).
4. Estimate battery voltage based on SOC.
5. Model simplified battery heat generation.
6. Simulate battery temperature.
7. Implement basic BMS safety monitoring.
8. Display battery information using a simple dashboard.

---

## 🛠️ Technologies Used

- Python
- NumPy
- Matplotlib
- Jupyter Notebook

---

## ⚙️ Features

### 🔋 State of Charge (SOC)

SOC represents the remaining charge in the battery.

The simulation calculates SOC based on:

- Battery capacity
- Charging/discharging current
- Time

### ❤️ State of Health (SOH)

SOH represents the estimated health of the battery compared with its original condition.

A simplified aging model is used to demonstrate how SOH decreases with battery cycles.

### ⚡ Voltage Estimation

Battery voltage is estimated using a simplified relationship between SOC and voltage.

### 🌡️ Thermal Model

The simulation calculates simplified heat generation using:

P = I²R

where:

- I = battery current
- R = internal resistance
- P = heat generation

A simplified temperature model is then used to simulate battery temperature.

### 🚨 BMS Safety Monitoring

The BMS checks:

- Low SOC
- Over-voltage
- Over-temperature

The system provides a basic status such as:

- NORMAL
- LOW SOC
- OVER VOLTAGE
- OVER TEMPERATURE

---

## 📊 Simulation Outputs

The project generates graphs for:

- SOC vs Time
- Voltage vs Time
- Temperature vs Time
- SOH vs Battery Cycles

It also provides a simple text-based BMS dashboard displaying the final battery condition.

---

## 🧠 Basic Working Principle

```text
                 Battery
                    |
                    ↓
              Current Input
                    |
        ┌───────────┼───────────┐
        ↓           ↓           ↓
       SOC       Heat I²R     Voltage
        |           |           |
        |           ↓           |
        |      Temperature      |
        |           |           |
        └───────────┼───────────┘
                    ↓
             BMS Safety Check
                    ↓
              BMS Dashboard