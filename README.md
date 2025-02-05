# EEG-Based ADHD Pattern Recognition  

## 📌 Reaserch Overview  
This project aims to identify recurring patterns in brain electrical activity among children with **Attention Deficit Hyperactivity Disorder (ADHD)** through EEG data analysis. The objective is to determine whether specific brain wave patterns can serve as **biological markers** for rapid and accurate ADHD diagnosis.  

## ⚙️ Methodology  
To achieve this goal, we preprocess and clean EEG signals using various signal processing techniques:  

- **High-pass and low-pass filtering** – to remove unwanted noise and improve signal clarity.  
- **Independent Component Analysis (ICA)** – to separate noise and artifacts from neural activity.  
- **Fast Fourier Transform (FFT)** – to analyze signal components in the frequency domain.  

After preprocessing, we analyze the patterns using the **Order Preserving Matching (OPM) algorithm**, which detects sequential structures while preserving relative order over time, regardless of absolute signal values.  

### 🔍 Pattern Analysis  
Our study explores these patterns using two main approaches:  

1. **Time Window Segmentation** – EEG signals are divided into time segments to assess recurring patterns over time.  
2. **Frequency Band Analysis** – Patterns are examined across different frequency bands to compare ADHD and control groups.  

A pattern is considered **ADHD-related** if:  
✅ It appears in at least **90% of cases within the ADHD group**.  
❌ It does **not appear similarly in the control group (NON-ADHD)**.  

A pattern that **does apear in the NON-ADHD group** is considered **ADHD-related** if:  
✅ It appears in at least **90% of cases within the NON-ADHD group**.
❌ It does **not appear similarly in the ADHD group at all(Emphasis on absolutely not!).**
 

## 🎯 Objectives and Impact  
The ultimate goal is to develop a model that facilitates **rapid and accurate ADHD identification** based on EEG data. These findings may contribute to:  

- 🏥 The development of an advanced **diagnostic tool** for early ADHD detection.  
- 📊 Improved personalization of **ADHD treatment strategies**.  

## 🚀 Future Work  
Potential extensions of this research include:  

- 🔹 **Incorporating another models** to enhance classification accuracy.  
- 🔹 **Expanding the dataset** to improve generalizability.  
- 🔹 **Investigating additional EEG features** that may provide further insights into ADHD diagnosis.  
