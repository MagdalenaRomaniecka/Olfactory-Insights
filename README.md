# Olfactory-Insights
An AI-powered perfume recommendation system that blends chemical note analysis (TF-IDF) with semantic understanding of fragrance descriptions (SBERT) to find your perfect scent match. Includes market segmentation via K-Means clustering.
# ✨ ScentSational: AI Perfume Recommender & Market Analysis

> *More than just notes—understanding the soul of a fragrance through NLP.*

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Libraries](https://img.shields.io/badge/Libs-Pandas%20|%20Scikit--Learn%20|%20SBERT%20|%20Streamlit-lightgrey)
![Status](https://img.shields.io/badge/Status-Complete-success)

## 🎯 Overview

Finding the perfect perfume is tough. Traditional recommenders only look at raw ingredients (e.g., "contains vanilla"), often missing the *vibe* or *mood* of a scent.

**ScentSational** solves this by building a **hybrid recommendation engine**. It combines hard data (chemical notes) with soft data (marketing descriptions) using advanced Natural Language Processing (NLP) to understand not just *what* a perfume is made of, but *how it feels* to wear it.

This project also includes a deep-dive market analysis, using unsupervised learning to automatically discover and map the 8 major "Scent Families" dominating the modern perfume landscape.

---

## 🔍 Key Features

* **👃 Hybrid Recommendation Engine:** Combines TF-IDF (for ingredient matching) with **Sentence-BERT (SBERT)** transformers (for semantic, contextual matching).
* **🧩 Automated Market Segmentation:** Uses **K-Means clustering** and PCA to discover hidden "Scent Families" without human labeling.
* **📊 In-Depth EDA:** Visual exploration of dominant brands, trending notes, and market structure.
* **🚀 Interactive Web App:** A fully functional Streamlit application for real-time testing (see `app.py`).

---

## 🛠️ Tech Stack

* **Data Processing:** `pandas`, `numpy`
* **Machine Learning:** `scikit-learn` (K-Means, PCA, TF-IDF, Cosine Similarity)
* **Deep Learning (NLP):** `sentence-transformers` (all-MiniLM-L6-v2)
* **Visualization:** `matplotlib`, `seaborn`, `wordcloud`
* **Deployment:** `streamlit`

---

## 📊 Insights & Visuals

### 1. Market Segmentation (The 8 Scent Families)
Using K-Means (k=8, determined via Elbow Method), I segmented 2,100+ perfumes into distinct families. The PCA visualization below shows clear clusters, separating fresh/citrus scents from heavy/oriental ones.

*(Place your `perfume_clusters_pca.png` here)*

### 2. The "DNA" of Popular Scents
What defines the current market? The analysis revealed a heavy dominance of warm, base-heavy notes like **Musk, Amber, and Vanilla**.

*(Place your `notes_wordcloud.png` here)*

### 3. Hybrid Model vs. Basic Model
Why use deep learning?
* **Basic Model (TF-IDF):** If you like *Vanilla*, it recommends *more Vanilla*. (Literal matching)
* **Hybrid Model (SBERT + TF-IDF):** If you like *Vanilla*, it might recommend a scent described as *"a warm, comforting hug on a winter day,"* even if it uses Tonka Bean instead of Vanilla. (Semantic matching)

---

## 🚀 Quick Start (Run Locally)

Want to test the recommender on your own machine?

1.  **Clone the repo:**
    ```bash
    git clone [https://github.com/YOUR-USERNAME/ScentSational.git](https://github.com/YOUR-USERNAME/ScentSational.git)
    cd ScentSational
    ```

2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the Streamlit app:**
    ```bash
    streamlit run app.py
    ```
    The app will open in your browser automatically!

---

## 📂 Repository Structure

* `perfume_analysis.ipynb` - Main Jupyter Notebook with all EDA, clustering, and model building steps.
* `app.py` - Streamlit application script for deployment.
* `perfumes_cleaned.csv` & `hybrid_similarity.npy` - Processed data files used by the app.
* `requirements.txt` - List of Python libraries needed to run the project.
* `/images` - Folder containing generated charts and visualizations.

---

## 📬 Contact

Created by ... - feel free to reach out on [LinkedIn](....) if you want to talk about data, perfumes, or AI!
