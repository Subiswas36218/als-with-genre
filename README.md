# 🎬 ALS vs ALS + Genres (MovieLens)

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg)

A **hybrid recommender system** that compares standard **Alternating Least Squares (ALS)** with an enhanced version incorporating **movie genre information** using the MovieLens dataset.

---

## 📌 Project Overview

This project explores how **content features (genres)** can improve collaborative filtering models.

We implement:

* 🎯 **Baseline ALS** (Matrix Factorization)
* 🎭 **ALS + Genre Integration** (Hybrid Model)

The goal is to evaluate whether incorporating genre metadata improves recommendation performance.

---

## 🧠 Key Concepts

* Collaborative Filtering
* Matrix Factorization (ALS)
* Hybrid Recommender Systems
* Feature Engineering (Genres)
* Evaluation Metrics (RMSE, Precision@K, Recall@K)

---

## 📂 Repository Structure

```
als-with-genre/
│── ALS_Genre_Project.ipynb   # Main notebook
│── README.md                 # Project documentation
│── data/                     # Dataset (optional / not uploaded)
│── results/                  # Plots and outputs
```

---

## 📊 Dataset

We use the **MovieLens dataset**, which contains:

* User ratings for movies
* Movie metadata including genres

🔗 Download: https://grouplens.org/datasets/movielens/

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/Subiswas36218/als-with-genre
cd als-with-genre
```

Install dependencies:

```bash
pip install numpy pandas matplotlib scikit-learn
```

---

## 🚀 Usage

Run the notebook:

```bash
jupyter notebook ALS_Genre_Project.ipynb
```

---

## 📈 Results

### 🔹 Metrics Used

* RMSE (Prediction Accuracy)
* Precision@K
* Recall@K

### 🔹 Observations

* ALS + Genres improves recommendation relevance
* Better ranking performance compared to baseline ALS
* Slight increase in computational complexity

---

## 📉 Visualizations

* Training Loss Curve
* Precision & Recall Comparison
* Genre Distribution Analysis

---

## 🎯 Sample Output

* Top-K movie recommendations for users
* Improved personalization using genre signals

---

## 🏗️ Methodology

1. Data preprocessing & ID mapping
2. Train-test split
3. ALS model training
4. Genre feature encoding
5. Hybrid model integration
6. Evaluation & comparison

---

## 🔮 Future Work

* Add deep learning models (Neural CF)
* Incorporate temporal dynamics
* Deploy as a web application
* Use larger datasets

---

## 👨‍💻 Author

**Subhankar Biswas**
MSc Data Engineering
Constructor University, Bremen, Germany

---

## 📜 License

This project is licensed under the MIT License.

---

## ⭐ Acknowledgements

* MovieLens Dataset (GroupLens Research)
* Recommender Systems literature
