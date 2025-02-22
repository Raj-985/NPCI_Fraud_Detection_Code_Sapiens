
# 🛡️ **UPI Fraud Detection System**  

An AI-based fraud detection system designed to identify fraudulent UPI transactions using machine learning. The system analyzes transaction patterns, user behaviors, and account balances to predict the likelihood of fraud in real-time.  

---

## 🚀 **Features**  
✅ High-accuracy fraud detection using machine learning  
✅ Real-time scalability for large datasets  
✅ Adaptable model with SMOTE for class imbalance  
✅ Performance evaluation using F1-Score (0.827)  

---

## 🧩 **Tech Stack**  
- **Programming Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-Learn, Imbalanced-Learn, Joblib  
- **Machine Learning Model:** Random Forest with SMOTE  
- **Deployment:** Docker & Streamlit (Single-file setup)  

---

## 📁 **Project Structure**  
```plaintext
UPI-Fraud-Detection
├── dataset/
│   ├── data.csv
├── model/
│   ├── fraud_detection_model.pkl
│   ├── scaler.pkl
├── app.py
├── train.py
├── test.py
├── requirements.txt
└── README.md
```

---

## ⚙️ **Setup and Installation**  

1. **Clone the Repository**  
```bash
git clone https://github.com/your-username/UPI-Fraud-Detection.git
cd UPI-Fraud-Detection
```

2. **Install Dependencies**  
```bash
pip install -r requirements.txt
```

3. **Train the Model**  
```bash
python train.py
```

4. **Test the Model**  
```bash
python test.py
```

5. **Run the Web Application**  
```bash
streamlit run app.py
```

---

## 💾 **Usage**  

1. Upload transaction data or enter values manually.  
2. The system will predict if the transaction is **Legitimate** or **Fraudulent**.  
3. Probability scores are provided to indicate the confidence level of predictions.  

---

## 🧠 **Machine Learning Workflow**  

- **Data Preprocessing:** Feature engineering, normalization, and handling class imbalance using SMOTE.  
- **Model Training:** Random Forest with hyperparameter tuning using RandomizedSearchCV.  
- **Prediction:** Real-time predictions with fraud probability scores.  
- **Performance Metrics:** Accuracy, Precision, Recall, and F1-Score (0.827).  

---

## ✅ **Performance**  

| **Metric**          | **Score**     |
|--------------------|--------------|
| **Accuracy**       | 0.91         |
| **Precision**      | 0.85         |
| **Recall**         | 0.81         |
| **F1-Score**       | 0.827        |

---

## 🐳 **Docker Deployment (Optional)**  
1. **Build Docker Image:**  
```bash
docker build -t upi-fraud-detection .
```

2. **Run Docker Container:**  
```bash
docker run -p 8501:8501 upi-fraud-detection
```

---

## 📝 **Contributing**  
Contributions are welcome! Feel free to submit a pull request or report issues.  

---

## 📜 **License**  
This project is licensed under the **MIT License**.  

---

## 💡 **Future Enhancements**  
🔹 Integrate XGBoost or LightGBM for faster predictions  
🔹 Use Neural Networks for detecting complex fraud patterns  
🔹 Add real-time API for production deployment  
