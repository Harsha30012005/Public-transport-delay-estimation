# Literature Review – Public Transport Delay Estimation Using Video Analytics and Vision Transformers

## 1. Introduction
Predicting public transport delays is critical for improving operational efficiency, passenger satisfaction, and transit planning. Traditional methods relying solely on GPS or schedule data often fail to capture real-world complexities such as traffic congestion, passenger boarding dynamics, and signal delays. Recent AI-based approaches have explored deep learning models using heterogeneous datasets, but gaps remain in **real-time performance, explainability, and multimodal integration**.  

This literature review examines key works relevant to delay prediction and highlights how they inform the proposed project.

---

## 2. Review of Related Works

### 2.1 DeepTTE: End-to-End Trajectory-based Travel Time Estimation (AAAI 2018)
- **Authors:** Wang et al.
- **Problem Addressed:** Predicts travel time using deep learning on GPS trajectory data.
- **Dataset & Methods:** Uses GPS trajectory sequences; employs multi-task deep neural network to predict segment and total travel time.
- **Key Findings:** Demonstrates strong performance on trajectory-based travel time estimation.
- **Limitations:** Focuses only on GPS data; lacks visual inputs and explainability.

---

### 2.2 Deep Learning Framework for Predicting Bus Delays Using Heterogeneous Datasets (ResearchGate 2020)
- **Authors:** Shoman et al.
- **Problem Addressed:** Predicts bus delays across multiple routes using GPS, schedule, and traffic data.
- **Dataset & Methods:** Heterogeneous datasets; deep learning models for network-wide delay estimation.
- **Key Findings:** Multisource data improves accuracy over GPS-only models.
- **Limitations:** Integration complexity; does not provide fine-grained visual explanations.

---

### 2.3 Wide & Deep Learning Models for Real-Time ETA Prediction (MDPI 2020)
- **Authors:** Zhang et al.
- **Problem Addressed:** Real-time Estimated Time of Arrival (ETA) prediction.
- **Dataset & Methods:** Combines linear (wide) models and deep neural networks.
- **Key Findings:** Hybrid architecture improves ETA prediction accuracy.
- **Limitations:** High computational requirement; still limited to tabular/temporal data.

---

### 2.4 DA-RNN: Dual-Stage Attention-Based Recurrent Neural Network (PMC 2020)
- **Authors:** Qin et al.
- **Problem Addressed:** Captures spatial-temporal dependencies in time series data.
- **Dataset & Methods:** Dual-stage attention RNN for feature selection and prediction.
- **Key Findings:** Attention improves predictive performance and highlights relevant features.
- **Limitations:** Complexity can lead to overfitting; lacks visual data integration.

---

### 2.5 Artificial Intelligence for Improving Public Transport: A Mapping Study (ResearchGate 2023)
- **Authors:** Jevinger et al.
- **Problem Addressed:** Surveys AI applications in public transport.
- **Dataset & Methods:** Systematic review categorizing AI studies by objectives and methods.
- **Key Findings:** AI can improve service quality, travel prediction, and resource allocation.
- **Limitations:** Broad survey; limited technical depth on specific models.

---

## 3. Comparative Summary

| Paper | Data Used | Model | Visual Inputs | Explainability | Real-Time | Limitations |
|-------|-----------|-------|---------------|----------------|-----------|-------------|
| DeepTTE (2018) | GPS | DNN | ❌ | ❌ | Partial | Only trajectory data |
| Deep Learning Heterogeneous (2020) | GPS, Schedule, Traffic | DNN | ❌ | ❌ | Partial | No video, complex integration |
| Wide & Deep (2020) | GPS & Tabular | Wide + DNN | ❌ | ❌ | ✔ | High computational cost |
| DA-RNN (2020) | Time Series | Attention RNN | ❌ | Partial | ✔ | Complexity, no video |
| AI Mapping Study (2023) | Survey | Multiple | ❌ | ❌ | N/A | Broad, lacks depth |

---

## 4. Synthesis & Research Gaps
While existing studies provide strong predictive frameworks using GPS and schedule data, **key gaps remain**:
1. **Multimodal Integration:** Visual inputs (traffic, signals, crowding) are not used.
2. **Explainability:** Delay predictions are not interpretable for passengers or authorities.
3. **Multi-Objective Outputs:** Most models focus only on ETA; reliability, waiting time, and ripple effects are rarely included.
4. **Real-Time Evidence:** No automated photo/video proof systems exist for accountability.

**Proposed Project Relevance:**  
Our approach combines **video analytics, GPS, and schedule data** with **Vision Transformers and Explainable AI** to produce **accurate, interpretable, multi-objective, and real-time delay predictions**, addressing all identified gaps.

---

### 5. Conclusion
The reviewed literature establishes a foundation for delay prediction using deep learning and heterogeneous data. The integration of **visual cues, temporal modeling, and explainable AI** represents a novel contribution that advances existing methods for smart public transport management.
