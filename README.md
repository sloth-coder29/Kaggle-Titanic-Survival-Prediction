# Kaggle - Titanic: Machine Learning from Disaster 

本專案針對 Kaggle Titanic 生存預測競賽，利用乘客基本資料（年齡、性別、票價、船艙等）進行**二元分類**，預測乘客是否存活。此專案著重於 **特徵工程流程建置**、**分類模型比較**與 **模型評估方法應用**。

---

##  專案內容

- 問題類型：二元分類（Survived vs Not Survived）
- 任務目標：透過乘客基本資料建立分類模型
- 訓練方式：整合前處理與模型訓練（Pipeline + ColumnTransformer）

---

## 方法應用

###  1. 特徵工程

| 特徵類型 | 處理方式 |
|----------|----------|
| 數值特徵（Age, Fare） | 缺失值以「中位數」填補 |
| 類別特徵（Sex, Embarked） | 填補缺失值，使用 `OneHotEncoder` 進行編碼 |
| 流程設計 | 使用 `Pipeline + ColumnTransformer` 整合特徵處理與模型訓練 |

---

###  2. 模型建立

| 模型 | 說明 |
|------|------|
| Logistic Regression | 基線模型，適合線性可分問題 |
| RandomForestClassifier | 較強模型，可處理複雜非線性關係 |

---

###  3. 模型評估方式

使用多元評估指標驗證模型效能：

- **Accuracy（準確率）**
- **混淆矩陣（Confusion Matrix）**
- **ROC-AUC 曲線**（區分能力）

---

##  成果表現

| 指標 | Logistic Regression | RandomForest |
|------|--------------------|--------------|
| Accuracy | ~0.804 | **~0.821** |
| ROC-AUC  | — | **0.84** |
| Kaggle Public LB | — | **0.75598** |

> RandomForest 在本專案中效果最佳，並展現出良好的分類判別能力。

---

