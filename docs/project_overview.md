# Public Transport Delay Estimation Using Video Analytics and Vision Transformers

## 📖 Abstract
Public transport delays caused by traffic, signals, and passenger boarding reduce reliability. Existing GPS-based systems give rough estimates but lack accuracy and clarity. This project proposes a deep learning framework that fuses video analytics, GPS, and schedule data for real-time bus delay prediction. CNNs and Vision Transformers process video to detect congestion, signals, and crowding, while sequence models estimate delays. The system provides explainable predictions, a passenger app with live alerts, and multi-objective outputs like waiting time and reliability. Future scope includes scaling citywide and integrating external factors for smarter transit planning.

---

## 🚧 Problem Statement
Public bus services often experience unpredictable delays due to traffic congestion, signal wait times, passenger boarding dynamics, and external factors such as weather and events. Current prediction methods, primarily based on GPS traces or schedule data, or using standard statistical and machine-learning models, fall short in several key respects:

1. They often provide coarse delay estimates without identifying the primary causes behind delays.  
2. They lack real-time responsiveness or adaptability to rapidly changing conditions.  
3. They typically target a single output delay rather than multiple performance metrics relevant to both passengers and transit authorities (e.g., reliability, passenger wait time, downstream impacts).  

---

## 🔍 Existing Solutions and Limitations

| Existing System | Method Used | Limitation |
|-----------------|--------------|-------------|
| **DeepTTE (AAAI 2018)** | Deep neural network on GPS trajectories | Ignores video data and lacks explainability |
| **Deep Learning on Heterogeneous Datasets** | Combines GPS, schedules, categorical data | No fine-grained visual insight into delays |
| **Embedding + Wide & Deep Models (MDPI 2020)** | Combines categorical + continuous features with attention | Some interpretability, no video analytics |
| **IoT + Neural Network Systems** | Predicts using GPS + schedule data | Limited to tabular data; no visual context |
| **Partitioned Sequence Models (DA-RNN, PMLNet)** | Divides travel into stages | Improved accuracy, but no visual reasoning |

---

## ❗ Gaps Identified
1. **Lack of Video Analytics:** Existing systems overlook visual cues such as congestion, passenger crowding, and signal states.  
2. **Limited Explainability:** Current models don’t quantify which factor (traffic, boarding, signals) caused a delay.  
3. **Single-Objective Focus:** Most predict only travel time, ignoring reliability or downstream effects.  
4. **Weak Real-Time Integration:** Systems rarely offer continuous updates or verifiable evidence of delays.  
5. **External Context Underuse:** Weather, events, and disruptions are not integrated into models.

---

## 🚀 Proposed Work

### 1. Video Analytics for Delay Factors  
- Use CNNs and Vision Transformers (ViTs) to analyze live or recorded camera feeds.  
- Detect congestion, signal states, and boarding events.  

### 2. Spatio-Temporal Delay Prediction  
- Fuse video, GPS, and schedule data using RNNs or Transformers.  
- Learn delay patterns in real time.  

### 3. Explainable AI (XAI) Module  
- Apply SHAP, Grad-CAM, and attention visualization to interpret model predictions.  
- Show factor contributions (e.g., 60% traffic, 30% signal, 10% boarding).  

### 4. Multi-Objective Real-Time Output  
- Predict multiple outputs: delay, reliability score, waiting time, ripple effects.  
- Update passengers and control centers continuously.  

### 5. Automated Photo Proof Sharing  
- Capture and share geo-tagged, time-stamped images during abnormal delays as verifiable proof for authorities.

---

## 🧩 Methodology Overview

| Step | Description |
|------|--------------|
| **Data Collection** | Gather synchronized video, GPS, and schedule data; label traffic, signal, and boarding events. |
| **Model Training** | CNN/ViT → detect congestion & crowd; Transformer → predict delay. |
| **Explainability** | Use Grad-CAM/SHAP to visualize contributing factors. |
| **Multi-Objective Testing** | Predict delay, reliability, waiting time, ripple effects. |
| **Photo Proof Module** | Auto-capture delay evidence; attach GPS + timestamp. |
| **Mobile App Prototype** | Display live delay alerts, alternate routes, and proof images. |

---

## 🧪 Experiments Planned

1. **Data Collection:** Build synchronized dataset of video, GPS, and schedule data.  
2. **Model Training:** Improve delay prediction accuracy over GPS-only baselines.  
3. **Explainability:** Use Grad-CAM/Attention maps to visualize causes of delay.  
4. **Multi-Objective Testing:** Evaluate metrics like reliability, waiting time, and ripple effects.  
5. **Photo Proof Module:** Auto-capture geo-tagged images for organizational use.  
6. **Mobile App Prototype:** Show real-time delays, confidence levels, and proof evidence.

---

## 🎯 Objectives

1. Integrate **video analytics, GPS, and schedule data** for accurate delay prediction.  
2. Implement **Explainable AI** for actionable insights.  
3. Output **multi-objective results** including reliability, passenger waiting time, and ripple effects.  
4. Build an **automated photo proof system** for verifiable evidence.  
5. Develop a **mobile application** for real-time alerts and alternate route suggestions.

---

## 📈 Expected Results

1. Scalable across multiple bus routes for citywide deployment.  
2. Integration of weather and event data for robust predictions.  
3. System evolves into a **digital twin** of urban transit for simulation.  
4. Advanced explainability for deeper insights into delay causes.  
5. Passenger app enhances trust via real-time proof and alerts.  
6. Integration with transport control centers for dynamic rerouting.

---

## 🔮 Future Scope
- Extend to multimodal transportation (metro, trams, taxis).  
- Introduce adaptive learning from live feedback.  
- Use edge AI for faster onboard camera analytics.  
- Integrate reinforcement learning for route optimization.

---

## 📘 Conclusion
This project builds an AI-powered framework that goes beyond conventional GPS-based delay prediction by combining **visual intelligence (video analytics)** with **temporal modeling** and **explainable AI**. The outcome is a **transparent, real-time, and multi-objective system** that benefits both passengers and transit authorities — paving the way for smarter, more reliable public transport systems.
