# 🪐 Exoplanet Detection Using Convolutional Neural Networks (CNNs)

### Overview
This project applies **deep learning** to automate the detection of **exoplanets** using light curve data from NASA’s **Kepler mission**.  
By analysing small dips in a star’s brightness — known as **transits** — the model identifies potential exoplanets orbiting distant stars.  

A **1D Convolutional Neural Network (CNN)** built with **PyTorch** was trained to classify whether a given light curve indicates a planetary transit or not.  
The project demonstrates how **AI can accelerate astronomical discovery** by efficiently processing large volumes of observational data.

---

### Objectives
- Detect planetary transits from light curve data using a CNN model.  
- Preprocess and normalise raw Kepler data for training and testing.  
- Evaluate model accuracy and interpret classification results.  
- Explore how AI can enhance large-scale data analysis in astronomy.  

---

### Key Components
- **Dataset:** [Kepler-labelled time-series data (Kaggle)](https://www.kaggle.com/datasets/keplersmachines/kepler-labelled-time-series-data)  
- **Model:** 1D CNN implemented in **PyTorch** for binary classification (*transit* vs *no transit*).  
- **Data Processing:** Noise reduction using the **Savitzky–Golay filter**, flux normalisation, and visual inspection of light curves.  
- **Performance:** Achieved **~99.12% accuracy** and **99.56% F1-score** on test data.  
- **Goal:** Improve the **efficiency and scalability** of exoplanet detection through deep learning.  

---

### Methodology
1. **Data Preprocessing**
   - Loaded and cleaned Kepler CSV data.  
   - Smoothed flux values using Savitzky–Golay filtering.  
   - Normalised and reshaped data into tensors suitable for CNN input.  

2. **Model Development**
   - Designed a 1D CNN with convolutional, pooling, and fully connected layers.  
   - Used **Binary Cross-Entropy Loss** and **Adam Optimiser** for training.  
   - Trained for 5 epochs using GPU runtime on Google Colab.  

3. **Evaluation**
   - Calculated Accuracy, Precision, Recall, and F1-score.  
   - Analysed the confusion matrix for false positives and class imbalance.  

---

### 📊 Results
| Metric | Value |
|--------|--------|
| **Accuracy** | 99.12% |
| **Precision** | 99.12% |
| **Recall** | 100% |
| **F1-Score** | 99.56% |

The CNN effectively detected exoplanet transits with high precision and recall, validating its capability to analyse complex astronomical data.

---

### Future Improvements
- Address **class imbalance** using SMOTE or weighted loss functions.  
- Apply the model to **TESS data** for generalisation testing.  
- Integrate **Explainable AI (XAI)** to interpret model predictions.  
- Expand to **multi-class classification** for other stellar variability types.  

---

### 🛠️ Tools & Technologies
`Python` • `PyTorch` • `NumPy` • `Pandas` • `SciPy` • `Matplotlib` • `Scikit-learn` • `Google Colab`

---

### 👩‍💻 Author
**Nikita Rawat**  
Bachelor of Computer & Information Sciences  
*(Major: Data Science | Minor: Astronomy & Space Science)*  
📍 Auckland, New Zealand  

---
