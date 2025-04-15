# Simulated Change-Point Detection in Poisson Count Data: A Physics-Inspired Approach
This project explores **change point detection** using two types of time series data:

1. **Simulated Poisson-distributed photon count data** with known change points  
2. **Real-world London weather data** (mean temperature & precipitation)

The aim is to identify structural changes in the time series that could indicate transitions, anomalies, or significant events — such as climate shifts or signal changes in scientific measurements.

---

##  Project Highlights

- Simulated change points using Poisson processes
- Custom z-score sliding window change point detection
- Applied to climate data (temperature and precipitation)
- Used `ruptures` for advanced detection on real-world data
- 📊 Visual comparisons of true and detected change points
- Precision, recall, and F1-score evaluation metrics


---

## Simulated Photon Count Data

We simulate a time series using Poisson distributions with step changes in the rate to represent change points (e.g., in photon emission rates).
A custom z-score based sliding window method is used to detect the change points.

## Real-World London Weather Analysis

We use the [London Weather Dataset from Kaggle](https://www.kaggle.com/datasets/emmanuelfwerr/london-weather-data).

### Key Features Analyzed:
- `mean_temp`: Mean daily temperature (°C)  
- `precipitation`: Daily rainfall (mm)

### Methods Applied:
- Our custom z-score based change point detection  
- `ruptures` library for advanced change point analysis  
- Preprocessing steps including:
  - Normalization
  - Log-scaling (for precipitation)

---

###  Visualization

Plots show:
- Raw time series data
- Detected change points (as vertical lines)
- Comparison of multiple methods

---

### 🧮 Evaluation Metrics

We use the following to evaluate detections:

- **True Positives (TP)**: Detected change points within a tolerance window of real change points  
- **False Positives (FP)**: Detections that don’t correspond to actual changes  
- **False Negatives (FN)**: Missed real change points

---

### Files

- `photon_counts.ipynb` – Main notebook  
- `requirements.txt` – Python dependencies  

---

