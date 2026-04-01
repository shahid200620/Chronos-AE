# ⏳ Chronos-AE: Time Series Anomaly Detection

A simple project that detects unusual patterns in time-series data using a convolution-based autoencoder model and visualizes results with Streamlit.

---

## 🚀 What this project does

This project learns how normal time-series data behaves and then identifies points where the behavior deviates.

Instead of using labels, the model learns patterns on its own and flags anything that looks different.

---

## 🧠 How it works (simple idea)

- Data is converted into small sequences (windows)
- A neural network tries to reconstruct these sequences
- If reconstruction error is high → it's likely an anomaly

---

## 🛠️ Tech used

- Python  
- NumPy, Pandas  
- PyTorch  
- Streamlit  
- Docker  

---

## 📂 Project Structure


scripts/ → preprocessing, training, evaluation
app/ → Streamlit dashboard
data/ → raw and processed data
models/ → saved model
results/ → output files
docs/ → explanation files


---

## ⚙️ How to run

### 1. Preprocess data

python scripts/preprocess_data.py


### 2. Train model

python scripts/train.py


### 3. Run evaluation

python scripts/evaluate.py


### 4. Launch dashboard

streamlit run app/main.py


---

## 📊 Output files

- anomaly_scores.csv  
- anomalies_percentile.csv  
- anomalies_pot.csv  
- streamlit_report.json  

---

## 📌 Notes

- Synthetic dataset is used to simulate real-world sensor data  
- Model is kept simple for clarity and stability  
- Focus is on complete pipeline rather than complexity  

---

## ✨ Final Thought

This project helped me understand how anomaly detection works without labels and how models can learn normal behavior from data.

It was interesting to see how small changes in data can lead to noticeable differences in reconstruction error.

---
