# 💵 Intelligent Banknote Verification using Machine Learning

This project demonstrates a practical application of **supervised machine learning** techniques to classify banknotes as **authentic** or **counterfeit** based on statistical features extracted from their scanned images. The solution is lightweight, interpretable, and ideal for embedded systems or real-time verification environments.

---

## 📁 Dataset Overview

- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/banknote+authentication)  
- **Format**: CSV (1372 samples, 5 columns)  
- **Features Extracted via**: Wavelet Transform on grayscale images of banknotes

| Feature        | Description                                   |
|----------------|-----------------------------------------------|
| Variance       | Variability of the wavelet-transformed image  |
| Skewness       | Asymmetry of image distribution               |
| Curtosis       | Sharpness and peakedness of image             |
| Entropy        | Information content or randomness             |
| Class          | 0 = Authentic, 1 = Forged                     |

---

## 🧠 Project Objective

To evaluate and compare various machine learning classification algorithms in terms of:
- **Accuracy**
- **Robustness** on small datasets
- **Speed** and computational simplicity
- **Real-time suitability**

---

## 🤖 Machine Learning Models Implemented

All models were implemented from scratch using NumPy and basic Python — **no auto ML libraries** were used in training the core classifiers.

- 🌳 **Decision Tree Classifier**  
- 🌲 **Random Forest Classifier**  
- 📍 **K-Nearest Neighbors (K = 3 and 5)**  
- ➖ **Support Vector Machine (SVM)**

---

## 📊 Performance Summary

| Model                    | Accuracy (%) |
|-------------------------|--------------|
| ✅ Decision Tree         | **99.27**    |
| 🌲 Random Forest         | 98.91        |
| 📍 KNN (k=3)             | 96.00        |
| 📍 KNN (k=5)             | 95.64        |
| ❌ Support Vector Machine| 41.82        |

📌 **Note**: Decision Tree emerged as the most reliable and interpretable model, achieving over **99%** accuracy on unseen data.

---

## 🧪 How to Run the Project

1. **Clone this repository:**
   ```bash
   git clone https://github.com/kanishka-mohankumar/BankNote-Authentication-ML.git
   cd BankNote-Authentication-ML
   ```

2. **Install required dependencies:**
   ```bash
   pip install numpy pandas matplotlib
   ```

3. **Run the main script:**
 

4. **Check the terminal output and generated plots for evaluation metrics.**

---

## 📌 Use Cases & Applications

This solution is adaptable to numerous real-world domains requiring rapid and reliable note verification:

- 🏦 **Banking Systems**
- 🏪 **Retail Point-of-Sale Machines**
- 🤖 **Automated Cash Handling Machines**
- 🎫 **Vending/Ticket Machines**
- 📱 **Mobile-Based Currency Verification Apps**

---

## 📈 Visualizations

The script includes:
- **Accuracy comparison bar chart**
- **Confusion matrix heatmaps**
- **Decision boundaries** (optional if matplotlib enabled)

---

## 🔍 Future Enhancements

- **Implement** logistic regression and Naive Bayes
- **Integrate** with mobile camera input for real-time detection
- **Add** Flask-based API for integration into web apps
- **Use** advanced ensemble techniques and cross-validation

---

## 🛠️ Tech Stack

- **Language**: Python
- **Libraries**: NumPy, Pandas, Matplotlib
- **ML Algorithms**: Custom-built classifiers
- **Testing**: Manual test cases and benchmarking

---

## 🪪 License

© 2025 – All Rights Reserved.

---

## 👨‍💻 Author

Created and maintained by [@kanishka-mohankumar](https://github.com/kanishka-mohankumar)

