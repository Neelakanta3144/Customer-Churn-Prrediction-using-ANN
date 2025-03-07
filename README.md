# **Customer Churn Prediction using ANN**

This project predicts customer churn using an **Artificial Neural Network (ANN)**. The dataset contains customer details and their churn status. The goal is to train an ANN model to classify whether a customer is likely to churn.


### **Want to make prediction**

**Deployed Link:** https://customer-churn-prrediction-using-ann-hxunomb6c9spykzvn2kms7.streamlit.app/
---

## 🚀 **Project Overview**

- **Dataset**: Customer dataset containing demographic and service-related features  
- **Model**: Artificial Neural Network (ANN) implemented using **TensorFlow/Keras**  
- **Goal**: Predict whether a customer will churn or not  

---

## 📂 **Project Structure**

```
📦 Customer-Churn-Prediction-using-ANN
│-- 📂 data                 # Dataset files (CSV)
│-- 📂 models               # Trained model and saved weights
│-- 📂 notebooks            # Jupyter notebooks for EDA and model training
│-- 📂 src                  # Source code for preprocessing and model training
│-- 📜 requirements.txt     # Python dependencies
│-- 📜 README.md            # Project documentation
│-- 📜 train.py             # Script to train the ANN model
│-- 📜 predict.py           # Script for making predictions
```

---

## ⚙️ **Installation & Setup**

1. **Clone the repository**  
   ```sh
   git clone https://github.com/Neelakanta3144/Customer-Churn-Prrediction-using-ANN.git
   cd Customer-Churn-Prediction-using-ANN
   ```

2. **Create a virtual environment (Optional but recommended)**  
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**  
   ```sh
   pip install -r requirements.txt
   ```

---

## 📊 **Dataset**

The dataset contains the following features:  
- **Customer Information**: Customer ID, Gender, Age, Tenure, etc.  
- **Subscription Details**: Services subscribed, Monthly & Total Charges  
- **Churn Label**: Whether the customer has churned or not  

---

## 🧠 **Model Architecture**

The ANN model consists of:  
- **Input Layer**: Accepts numerical and categorical features  
- **Hidden Layers**: Multiple dense layers with activation functions  
- **Output Layer**: Single neuron with Sigmoid activation (binary classification)  

```python
model = Sequential([
    Dense(64, activation='relu', input_shape=(num_features,)),
    Dropout(0.3),
    Dense(32, activation='relu'),
    Dense(1, activation='sigmoid')  # Binary classification
])
```

---

## 🚀 **How to Train the Model?**

Run the training script:  
```sh
python train.py
```
This will:
- Preprocess the data  
- Train the ANN model  
- Save the trained model  

---

## 🔍 **Making Predictions**

Use the `predict.py` script to predict churn for new customers.  
```sh
python predict.py --input "new_customer_data.csv"
```


## 📜 **License**

This project is open-source under the **MIT License**.  

---

