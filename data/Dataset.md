# 📂 Dataset Documentation

This project uses the **MovieLens dataset**, a widely used benchmark dataset for recommender systems research.

---

## 📌 Dataset Overview

The dataset contains:

* User ratings for movies
* Movie metadata including titles and genres

It is maintained by **GroupLens Research** at the University of Minnesota.

🔗 Official Source: https://grouplens.org/datasets/movielens/

---

## 📊 Dataset Files Used

### 1. `ratings.csv`

Contains user interactions with movies.

| Column    | Description                    |
| --------- | ------------------------------ |
| userId    | Unique user identifier         |
| movieId   | Unique movie identifier        |
| rating    | Rating given by user (0.5–5.0) |
| timestamp | Time of rating                 |

---

### 2. `movies.csv`

Contains movie metadata.

| Column  | Description                                 |
| ------- | ------------------------------------------- |
| movieId | Unique movie identifier                     |
| title   | Movie title                                 |
| genres  | Pipe-separated genres (e.g., Action|Comedy) |

---

## 🎭 Genre Information

Genres are provided as categorical labels such as:

* Action
* Comedy
* Drama
* Thriller
* Romance

### Encoding Strategy

* Extract unique genres
* Create a genre index mapping
* Convert genres into **multi-hot vectors**

This allows integration into the hybrid ALS model.

---

## 🔄 Preprocessing Steps

1. Remove missing or invalid entries
2. Map `userId` and `movieId` to continuous indices
3. Split dataset into:

   * Training set (80%)
   * Test set (20%)
4. Normalize or directly use ratings depending on model design

---

## 📈 Dataset Characteristics

* Sparse user-item interaction matrix
* Long-tail distribution of movies
* Users typically rate a small subset of items

These properties make it suitable for testing recommender systems.

---

## ⚠️ Notes

* The dataset is **not included** in this repository due to size constraints
* Please download it manually from the official source

---

## 🚀 How to Use

1. Download the dataset
2. Extract files
3. Place them inside:

```id="3z6wd6"
data/
```

Expected structure:

```id="q0r0sh"
data/
├── ratings.csv
├── movies.csv
```

---

## 📜 License

The MovieLens dataset is available for research purposes.
Refer to the official website for licensing details.

---

## ✅ Summary

The MovieLens dataset provides:

* Real-world user behavior
* Rich metadata (genres)
* A standard benchmark for evaluating recommender systems

It is ideal for comparing **collaborative filtering vs hybrid models**.
