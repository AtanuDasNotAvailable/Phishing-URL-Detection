# 🛡️ PHI-ISIIL Phishing URL Dataset

## 📖 Overview
The **PHI-ISIIL Phishing URL Dataset** is a publicly available dataset designed for research in cybersecurity, specifically for detecting phishing websites. It contains labeled URLs categorized as either **phishing** or **legitimate**, making it suitable for training and evaluating machine learning models.  

---

## 🌐 Dataset Source
- **Original Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/967/phiusiil+phishing+url+dataset)  
- **Contributors:** Safaa Zareapoor and Abdullah Gani  
- **Domain:** Cybersecurity, Machine Learning, Phishing Detection

---

## 📊 Dataset Description
The dataset includes URLs with features that help distinguish phishing sites from legitimate ones:  

- **🔗 URL-based features:** Characteristics derived from the URL’s structure and composition  
- **🏷️ Domain-based features:** Domain info, including age, DNS records, and WHOIS details  
- **💻 Content-based features:** Features extracted from HTML and JavaScript

---

## 📂 Data Format
The dataset is provided in **CSV format** with the following columns:  

- `URL` 🌐 – The web address being analyzed  
- `Features` 🧩 – Numerical and categorical attributes extracted from the URL and web content  
- `Label` 🏷️ – Binary classification label:
  - `0` → **Legitimate** website ✅  
  - `1` → **Phishing** website ⚠️

---

## 🚀 Usage
This dataset can be used for:  

- 🧠 Training and testing ML models for phishing detection  
- 🛠️ Feature engineering and selection to improve classification performance  
- 📊 Benchmarking cybersecurity approaches for phishing prevention

---

## ⚡ How to Use

### 1️⃣ Download the Dataset
- Clone this repository or manually download the CSV file  
- Or fetch the dataset directly from the [UCI Repository](https://archive.ics.uci.edu/dataset/967/phiusiil+phishing+url+dataset)

### 2️⃣ Load the Dataset in Python
```python
import pandas as pd

# Load dataset
df = pd.read_csv('PHI_ISIIL_Phishing_URL_Dataset.csv')

# Display first few rows
print(df.head())
 ```

3️⃣ Train a Machine Learning Model
```python
from sklearn.model_selection import train_test_split
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import accuracy_score

# Split data
X = df.drop(columns=['URL', 'Label'])
y = df['Label']
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

# Train model
model = RandomForestClassifier()
model.fit(X_train, y_train)

# Evaluate model
y_pred = model.predict(X_test)
print("Accuracy:", accuracy_score(y_test, y_pred))
 ```

📚 Citation
```python
@misc{phiisiil2023,
  title={PHI-ISIIL Phishing URL Dataset},
  author={Safaa Zareapoor and Abdullah Gani},
  year={2023},
  url={https://archive.ics.uci.edu/dataset/967/phiusiil+phishing+url+dataset}
}
 ```

⚖️ License

This dataset is provided for research purposes. Please refer to the original source for licensing details.
This repository serves as a resource to help combat cyber threats using machine learning techniques. Happy coding! 🚀


---

