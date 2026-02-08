<div align="center">

# 💖 Heart Disease Prediction

![Python](https://img.shields.io/badge/python-3.8+-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-1.3.0-orange.svg)
![Streamlit](https://img.shields.io/badge/streamlit-1.25.0-red.svg)
![Accuracy](https://img.shields.io/badge/accuracy-86.41%25-success.svg)

**A machine learning application for predicting heart disease using multiple ML algorithms**

[Demo](#-usage) • [Features](#-features) • [Installation](#-installation) • [Dataset](#-dataset) • [Models](#-model-performance)

[![GitHub](https://img.shields.io/badge/GitHub-Saksham-black?style=for-the-badge&logo=github)](https://github.com/Dumbsham)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Saksham-blue?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/saksham14sharma)

</div>

---

## 🎯 Overview

This project uses patient health metrics to predict the likelihood of heart disease. Built with Python and scikit-learn, the application compares multiple machine learning algorithms to provide accurate heart disease predictions through an interactive web interface.

## ✨ Features

- 🤖 **Multiple ML Models**: Comparison of Logistic Regression, KNN, Naive Bayes, Decision Trees, and SVM
- 🔄 **Smart Preprocessing**: Automated data cleaning, feature scaling, and encoding
- 🖥️ **Interactive Web App**: User-friendly Streamlit interface for real-time predictions
- 📊 **Comprehensive EDA**: Detailed exploratory data analysis with visualizations
- 💾 **Model Persistence**: Pre-trained models ready for deployment
- 🎯 **High Accuracy**: Best model achieves 86.96% accuracy

## 📁 Project Structure
```
heart-disease-prediction/
├── 📄 app.py              # Streamlit web application
├── 📁 data/
│   ├── heart.csv          # Training dataset (918 samples)
│   └── columns.pkl        # Feature columns metadata
├── 📁 models/
│   ├── KNN_heart.pkl      # Trained KNN model
│   └── scaler.pkl         # StandardScaler for normalization
├── 📁 notebooks/
│   └── heart.ipynb        # EDA and model training notebook
├── 📄 requirements.txt    # Python dependencies
├── 📄 README.md          # Project documentation
└── 📄 LICENSE            # MIT License
```

## 🚀 Installation

1. **Clone the repository:**
```bash
git clone https://github.com/yourusername/heart-disease-prediction.git
cd heart-disease-prediction
```

2. **Create a virtual environment:**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies:**
```bash
pip install -r requirements.txt
```

## 💻 Usage

### Running the Application
```bash
streamlit run app.py
```

The application will open in your browser at `http://localhost:8501`

### 🩺 Input Features

The application accepts the following patient health metrics:

| Feature | Description | Type |
|---------|-------------|------|
| 👤 **Age** | Patient age in years | Numeric |
| ⚥ **Sex** | M (Male) or F (Female) | Categorical |
| 💔 **Chest Pain Type** | ATA, NAP, ASY, TA | Categorical |
| 🩸 **Resting BP** | Resting blood pressure (mm Hg) | Numeric |
| 🧪 **Cholesterol** | Serum cholesterol (mg/dL) | Numeric |
| 🍬 **Fasting BS** | Fasting blood sugar > 120 mg/dL | Binary |
| 📊 **Resting ECG** | Normal, ST, LVH | Categorical |
| ❤️ **Max HR** | Maximum heart rate achieved | Numeric |
| 🏃 **Exercise Angina** | Exercise-induced angina (Y/N) | Binary |
| 📉 **Oldpeak** | ST depression induced by exercise | Numeric |
| 📈 **ST Slope** | Slope of peak exercise ST segment | Categorical |

## 📊 Model Performance

Multiple machine learning algorithms were trained and evaluated:

| Model | Accuracy | F1-Score | Status |
|-------|----------|----------|--------|
| **Logistic Regression** | **86.96%** | **88.46%** | 🥇 Best Overall |
| **K-Nearest Neighbors** | **86.41%** | **88.15%** | ⭐ Deployed |
| **Support Vector Machine** | 84.78% | 86.67% | ✅ Good |
| **Naive Bayes** | 84.78% | 86.14% | ✅ Good |
| **Decision Trees** | 79.35% | 80.61% | ⚠️ Baseline |

> **Note:** KNN was chosen for deployment due to its excellent balance of accuracy and interpretability.

### 🔬 Data Preprocessing

- ✅ Handled missing values (Cholesterol & RestingBP zeros replaced with mean)
- ✅ One-hot encoding for categorical variables
- ✅ StandardScaler normalization for numerical features
- ✅ Train-test split: 80-20
- ✅ No duplicate records found

## 📈 Dataset

- **Source:** [Heart Disease Dataset](https://github.com/AkarshVyas/Machine-Learning-Part-1/blob/main/heart.csv)
- **Samples:** 918 patient records
- **Features:** 11 clinical features + 1 target variable
- **Target Distribution:** Balanced dataset (HeartDisease: 0/1)

### Sample Data
```
Age  Sex  ChestPainType  RestingBP  Cholesterol  ...  HeartDisease
40   M    ATA            140        289          ...  0
49   F    NAP            160        180          ...  1
37   M    ATA            130        283          ...  0
```

## 🛠️ Technologies Used

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

</div>

- **Machine Learning:** scikit-learn (Logistic Regression, KNN, Naive Bayes, Decision Trees, SVM)
- **Data Processing:** pandas, numpy
- **Visualization:** matplotlib, seaborn
- **Web Framework:** Streamlit
- **Model Serialization:** joblib

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. 🍴 Fork the repository
2. 🔧 Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. 💾 Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. 📤 Push to the branch (`git push origin feature/AmazingFeature`)
5. 🔃 Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- 💡 Inspired by healthcare machine learning applications
- 🎓 Built as a learning project in ML and web development

## 📧 Contact

<div align="center">

**Your Name**

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Dumbsham)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/saksham14sharma)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sakshamnoida37@gmail.com)

⭐ Star this repository if you found it helpful!

</div>

---

<div align="center">
Made with ❤️ and Python
</div>
