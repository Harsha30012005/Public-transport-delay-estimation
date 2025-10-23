# Research Questions – Public Transport Delay Estimation Using Video Analytics and Vision Transformers

The following research questions guide the design, experimentation, and validation of this project.

---

### 🎯 Core Questions

| No. | Research Question | Purpose |
|-----|--------------------|----------|
| 1 | How effectively can Vision Transformers (ViTs) and CNNs extract delay-related features such as congestion, signal status, and passenger density from real-world video data? | To benchmark visual feature extraction quality |
| 2 | What is the optimal fusion strategy (early, mid, or late fusion) for combining video, GPS, and schedule data to improve prediction accuracy? | To design a robust multimodal integration framework |
| 3 | How do temporal models like LSTM and Transformers compare in capturing spatio-temporal dependencies for delay estimation? | To identify the best-performing sequence model |
| 4 | How can explainable AI techniques (SHAP, Grad-CAM, attention visualization) make the delay prediction interpretable to passengers and transport authorities? | To ensure transparency and trust in model predictions |
| 5 | Which delay factors (traffic, signals, boarding time, weather) contribute most to overall delay variability, and how can these be quantified? | To prioritize impactful variables for intervention |
| 6 | How well can the model generalize to unseen routes and real-time scenarios across different cities? | To test scalability and robustness |
| 7 | How does incorporating external contextual data (weather, events, disruptions) affect prediction stability and adaptability? | To evaluate multi-context learning performance |
| 8 | Can the automated photo proof module enhance credibility and decision-making for transport organizations? | To validate real-world utility and accountability |

---

### 🧩 Research Hypotheses

1. Integrating video analytics with GPS and schedule data will **significantly outperform GPS-only systems** in delay prediction accuracy.  
2. Vision Transformers will capture **richer visual delay features** (e.g., congestion density, signal wait times) than CNN baselines.  
3. Multi-objective outputs (delay, reliability, waiting time) will improve operational insights compared to single-output models.  
4. Explainability methods will enhance **trust and interpretability**, increasing system acceptance by authorities.  
5. The automated proof module will offer **verifiable, timestamped visual evidence**, improving transparency in public reporting.

---

### 🧠 Expected Outcomes
- A validated hybrid deep learning model integrating video and GPS data.  
- Clear identification of top factors contributing to bus delays.  
- Explainable, real-time predictions deployable in passenger applications.  
- Benchmark comparisons with existing baselines like DeepTTE and DA-RNN.

---

### 🗂️ References for Research Direction
1. Li, Y. et al., *DeepTTE: End-to-End Trajectory-based Travel Time Estimation*, AAAI 2018.  
2. Zhang, J. et al., *Deep Learning on Heterogeneous Datasets for Bus Delay Prediction*, IEEE Transactions on ITS.  
3. Chen, Z. et al., *Wide & Deep Learning Models for Real-Time ETA Prediction*, MDPI 2020.  
4. Xiao, Y. et al., *DA-RNN: Dual-Stage Attention-Based Recurrent Neural Networks*, 2017.  

---


