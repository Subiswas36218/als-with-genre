# 📊 Plots and Visualizations

This document presents the key visualizations generated in the **ALS vs ALS + Genres** recommender system project.

---

## 📉 1. Training Loss Curve

### Description

This plot shows how the training loss decreases over iterations for both:

* Baseline ALS
* ALS with Genre Integration

### Insight

* Convergence behavior of both models
* Stability of optimization
* Faster or smoother convergence indicates better training dynamics

### Expected Observation

ALS + Genres may converge more smoothly due to additional information.

---

## 📊 2. Precision@K Comparison

### Description

A bar chart comparing Precision@K for:

* ALS
* ALS + Genres

### Insight

* Measures how many recommended items are relevant
* Higher precision → better recommendation quality

### Expected Observation

Hybrid model typically achieves higher precision.

---

## 📊 3. Recall@K Comparison

### Description

A bar chart comparing Recall@K for both models.

### Insight

* Measures how many relevant items are successfully recommended
* Higher recall → better coverage

### Expected Observation

ALS + Genres improves recall due to richer feature representation.

---

## 📉 4. Error Distribution

### Description

Histogram of prediction errors for:

* ALS
* ALS + Genres

### Insight

* Spread of prediction errors
* Detects bias or variance issues

### Expected Observation

Hybrid model should show tighter error distribution.

---

## 🎭 5. Genre Distribution

### Description

Histogram showing number of genres per movie.

### Insight

* Dataset diversity
* Helps understand feature richness

### Expected Observation

Most movies have 1–3 genres.

---

## 🔁 6. Convergence Comparison

### Description

Overlayed loss curves comparing:

* ALS
* ALS + Genres

### Insight

* Direct comparison of learning efficiency
* Helps evaluate model robustness

---

## 📌 Notes

* All plots are generated using **Matplotlib**
* Ensure consistent scaling for fair comparison
* Use proper labels and legends for clarity

---

## 🚀 How to Reproduce Plots

Run the notebook:

```bash
jupyter notebook ALS_Genre_Project.ipynb
```

All plots will be generated automatically.

---

## 📂 Optional: Save Plots

To save plots, add:

```python
plt.savefig("results/plot_name.png")
```

Store them inside:

```
results/
```

---

## ✅ Summary

These visualizations help:

* Compare model performance
* Understand training dynamics
* Validate improvements from genre integration
