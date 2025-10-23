# 🚌 Public Transport Delay Estimation Using Video Analytics and Vision Transformers

### 🚀 Overview
This project proposes a deep learning framework that predicts **bus delays in real-time** by fusing **video analytics, GPS, and schedule data**.  
Unlike traditional GPS-only systems, it leverages **Vision Transformers (ViTs)** and **Explainable AI** to analyze traffic, signal conditions, and passenger boarding activities for more accurate and transparent delay predictions.

---

### 📖 Abstract
Public transport delays caused by traffic, signals, and passenger boarding reduce reliability. Existing GPS-based systems give rough estimates but lack accuracy and clarity.  
This project introduces a **hybrid AI model** that uses CNNs and Vision Transformers to extract visual insights (traffic congestion, signals, crowding) and sequence models (RNNs/Transformers) to predict delays.  
The framework provides explainable predictions, live passenger alerts, and multi-objective outputs like **reliability score, waiting time, and ripple effects**.  
Future extensions include scaling citywide and integrating weather and event data for **smarter urban transit planning**.

---

### 🎯 Objectives
- Integrate **video analytics, GPS, and schedule data** for precise bus delay prediction.  
- Provide **explainable outputs** showing contribution of traffic, signals, and passenger crowding.  
- Predict multiple performance metrics — **delay, reliability, waiting time, and ripple effects.**  
- Enable **real-time proof generation** through geo-tagged images and timestamps.  
- Build a **passenger mobile app** for delay alerts, confidence levels, and alternate route suggestions.

---

### 🧠 Methodology

| Stage | Description |
|--------|--------------|
| **1. Video Analytics** | Use CNNs and Vision Transformers (ViTs) to detect congestion, signal states, and boarding activities. |
| **2. Spatio-Temporal Prediction** | Fuse visual, GPS, and schedule data using RNNs/Transformers for temporal learning. |
| **3. Explainability Module** | Use SHAP and Grad-CAM to show which factors influenced the delay prediction. |
| **4. Real-Time Multi-Objective Output** | Predict delay, reliability, and waiting time continuously. |
| **5. Proof & App Integration** | Auto-capture images and push results to a mobile app with live notifications. |

---

### 📊 Expected Outcomes
- 15–25% improvement in accuracy over GPS-only models.  
- Visual detection of **congestion**, **signal state**, and **crowding**.  
- Explainable results showing **factor-wise contribution** to delays.  
- Real-time updates for passengers and control centers.  
- Proof generation module for verified delay evidence.

---

### 🧪 Experiments Planned
1. Collect synchronized datasets (video, GPS, schedule).  
2. Train CNNs/ViTs for visual event detection.  
3. Develop RNN/Transformer model for delay prediction.  
4. Integrate XAI (SHAP/Grad-CAM) for interpretability.  
5. Build a prototype mobile dashboard for real-time outputs.  

---

### 🧩 Folder Structure
