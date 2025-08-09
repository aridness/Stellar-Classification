# 🌌 Stellar Classification — Stars, Galaxies, and Quasars

This machine learning project classifies **stars**, **galaxies**, and **quasars** based on the [Sloan Digital Sky Survey DR17](https://www.kaggle.com/datasets/fedesoriano/stellar-classification-dataset-sdss17/data) dataset.

> Developed as part of a project at **Università degli Studi di Pavia** by *Ariele Mairani*.

![unipv logo](unipv-logo.png)

---

## 📄 Project Overview
The aim of this project is to explore supervised machine learning pipelines, through astronomical object classification.  
We:
- Perform **data preprocessing** and handle class imbalance.
- Explore different **dimensionality reduction** techniques (PCA, LDA).
- Train and compare multiple classifiers.
- Evaluate model performance using **F1-score**, **precision**, and **confusion matrices**.

---

## 📊 Dataset
- **Source:** [Kaggle — Stellar Classification Dataset (SDSS17)](https://www.kaggle.com/datasets/fedesoriano/stellar-classification-dataset-sdss17/data)  
- **Content:** Photometric measurements, redshift, and other astronomical features from the SDSS DR17.  
- **Target:** `class` — one of `GALAXY`, `STAR`, `QSO` (quasar).

---

## 🛠 Methods & Tools
**Languages & Libraries**
- Python — `pandas`, `numpy`, `scikit-learn`, `imblearn`, `matplotlib`, `seaborn`
- Feature selection with **SFS** (Sequential Feature Selector)
- Class balancing with **SMOTE** and undersampling

**Models Tested**
- Logistic Regression
- Random Forest Classifier
- Perceptron

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/stellar-classification.git
   cd stellar-classification
2. Install dependencies
   ```bash
   pip install -r requirements.txt
3. Run the notebook. The Cross Validation will take hours, so pre-calculated values are already present in the `cv_results_upload.pkl` file. To use them simply skip the `scores = cross_validate()` cell and the `with open("cv_results.pkl", "wb") as f:` cell. 
    ```bash
   jupyter notebook main.ipynb


## 📈 Results

**Best model:** Random Forest Classifier  
- **F1-score train:** _0.9758_  
- **F1-score test:** _0.9817_  

---

## 📬 Contact

- **Author:** Ariele Mairani  
- **GitHub:** https://github.com/aridness
- **LinkedIn:** www.linkedin.com/in/ariele-mairani-59bba6343  
- **Email:** ari.mairani@gmail.com

---

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for the full text.

