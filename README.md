# Kaggle - Titanic Survival Prediction

本專案參與 Kaggle 經典競賽 **Titanic - Machine Learning from Disaster**，透過資料清理、特徵工程以及多模型 Stacking Ensemble（`Logistic Regression + Random Forest`）預測乘客是否存活。

---

## Kaggle 成績

| 指標 | 分數 |
|------|------|
| **Public LB (Accuracy)** | **0.756** |
| **模型架構** | Logistic Regression + Random Forest |
| **資料處理** | 缺值填補、特徵工程、One-Hot Encoding |

---

##  使用工具

- Python
- Pandas, NumPy
- Scikit-Learn
- Matplotlib / Seaborn (視覺化)
- Jupyter Notebook

---

## 專案流程

```text
資料讀取與清理
       ↓
特徵工程（缺值填補、編碼處理）
       ↓
模型訓練（Logistic Regression / Random Forest）
       ↓
Stacking Ensemble
       ↓
模型評估與提交

