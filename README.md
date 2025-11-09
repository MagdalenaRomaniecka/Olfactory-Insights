# 📈 Olfactory-Insights: A Deep Dive into Perfume Market Data

## 🚀 View the Live Application!
**The insights from this Exploratory Data Analysis (EDA) were used to build a fully deployed AI perfume recommender application.**

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://scentsational-evywcwtgnrevjgm4ubxappy.streamlit.app/)

[**➡️ Click here to try the "ScentSational" app**](https://scentsational-evywcwtgnrevjgm4ubxappy.streamlit.app/)

---

## 🎯 Project Goal

This repository contains a detailed **Exploratory Data Analysis (EDA)** of the niche perfume market. The goal was to understand market structures, identify key trends, and prepare the data for building a recommendation model.

This analysis served as the foundational research for the [ScentSational (AI Recommender)](https://github.com/MagdalenaRomaniecka/ScentSational) project.

---

## 🔑 Key Analytical Insights

The `EDA.ipynb` notebook contains the full process, but here are the key findings:

* **Market Leaders:** A frequency analysis revealed the market is dominated by key niche brands, with **Tom Ford Private Blend, Profumum, and Serge Lutens** leading the pack.
* **Core Ingredients:** The most common notes across the entire dataset are **Musk, Rose, and Vanilla**.
* **Market Segmentation:** Using K-Means (k=8), **8 distinct "Scent Families"** were identified from the data.
* **Marketing Strategy:** Interestingly, the analysis showed that marketing description length is very similar across all clusters, peaking between 150-175 words.

---

## 🛠️ How to Run This Analysis

1.  Clone the repository:
    ```bash
    git clone [https://github.com/MagdalenaRomaniecka/Olfactory-Insights.git](https://github.com/MagdalenaRomaniecka/Olfactory-Insights.git)
    cd Olfactory-Insights
    ```
2.  Install the required libraries:
    ```bash
    pip install -r requirements.txt
    ```
3.  Run Jupyter Notebook:
    ```bash
    jupyter notebook EDA.ipynb
    ```

---

## 📦 Tech Stack

* **Data Analysis:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn, WordCloud
* **Modeling (EDA):** Scikit-learn (K-Means, PCA)
* **Environment:** Jupyter Notebook
