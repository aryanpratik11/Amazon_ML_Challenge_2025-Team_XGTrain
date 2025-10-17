# Price Prediction based on given dataset — Amazon ML Challenge 2025

**Machine learning pipeline for predicting product prices based on a shabby dataset (text clusters + images)** developed for the **Amazon ML Challenge 2025**.

This repository collects the full pipeline we built during the hackathon:
- data cleaning & unit standardization
- quantity extraction from product text
- outlier handling (removal + winsorization)
- DistilBERT text embeddings for product titles/descriptions
- image processing pipeline
- XGBoost regression model with hyperparameter tuning
- training & inference scripts, plus result artifacts

---

## Quick start

1. Clone the repository:
```bash
git clone https://github.com/aryanpratik11/Amazon_ML_Challenge_2025-Team_XGTrain.git
cd Amazon_ML_Challenge_2025-Team_XGTrain
```
2. Create a Python environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```
3. Place data
   - Put original CSVs(train.csv, test.csv) in the root folder
   - Run the train_clean.ipynb and test_clean.ipynb to get a cleaner and more structured versions of original dataset

---

## Results achieved
  - Final reported metric: SMAPE: 52.56% (best run from tuning)
  - Placed the team in top 20% of the leaderboard


---

## Notes & reproducibility
  - The dataset used in the hackathon contained noisy textual clusters and product images; all heavy binary files (images, embeddings, model binaries) are excluded from the repo and should be downloaded separately

---

### 👨‍💻 Team Members
- [**Aryan Pratik**](https://github.com/aryanpratik11)
- [**Pavan Kumar**](https://github.com/pavan)
