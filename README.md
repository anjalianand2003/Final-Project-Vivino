# Final-Project-Vivino
# 🍷 Vivino Wine Quality Classification

This project uses machine learning to classify French Bordeaux wines as **"poor," "okay," or "good"** based on physicochemical properties. Developed as a final academic project, it supports **Vivino's marketing and recommendation strategy** using robust predictive models.

## 📁 Project Files

- `vivino_wine_quality_classification.R` – Complete classification workflow
- `vivinoQuality.csv` – Input dataset (1599 wine samples)
- `README.md` – Project documentation

---

## 📊 Dataset Overview

- **Samples:** 1599 French Bordeaux wines
- **Features:** 11 physicochemical properties (e.g., alcohol, density, acidity)
- **Target Variable:** `quality2` – categorized as `poor`, `okay`, or `good`

---

## 🔍 Objectives

- Build classification models to predict wine quality
- Evaluate feature importance for marketing
- Support Vivino’s product strategy through data insights

---

## 🧠 Methods Used

| Model           | Accuracy | Highlights |
|----------------|----------|------------|
| Naive Bayes     | 98%      | Efficient but struggles with overlapping classes |
| Random Forest   | 100%     | Highly robust with perfect classification accuracy |
| Balanced RF     | 100%     | Handles class imbalance effectively |

---

## 🔬 Feature Importance

- **Top Predictors:** `Alcohol`, `Sulphates`, and `Density`
- **Visualization:** Heatmaps, Corrplots, and Component Scatterplots
- **Business Insight:** Wines high in alcohol and sulphates are high quality

---

## 📈 Visualizations

- Cluster plots for predicted classes
- Heatmap of feature importance
- Correlation matrix of variables

---

## 🎯 Business Applications for Vivino

1. **Targeted Promotions:** Emphasize high-alcohol, low-density wines
2. **Production Partnerships:** Guide winemakers on ideal profiles
3. **Personalization:** Integrate the model into Vivino's recommendation engine

---

## 💻 How to Run

```r
install.packages(c("tidyverse", "caret", "randomForest", "e1071", "cluster", "mclust", "gplots", "RColorBrewer", "corrplot"))
source("vivino_wine_quality_classification.R")
