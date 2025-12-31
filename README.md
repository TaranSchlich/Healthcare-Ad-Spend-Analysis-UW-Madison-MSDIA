# Healthcare Ad Spend Analysis
**By: Taran Schlichtmann**

**Date: 10/14/2025**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1biipk8rwW8KrbrZhNZHAfXt8hH-7khL1)

---

## Business Context
Analyze advertising effectiveness by predicting sales from TV, radio, and newspaper spend. Use Python for data exploration, correlation analysis, and linear regression modeling to provide insights for optimizing marketing investments.

---

## Learning Objectives
- Perform **data exploration** and **visualization**.
- Compute **correlations** between advertising channels and sales.
- Build and evaluate a **linear regression model**.

---

## Repository Structure
```
.
├── gb881_assignment_6_schlichtmann_t.py   # Core analysis script
└── README.md                               # Project documentation
```

---

## Tech Stack
- Python 3.x
- Pandas — Data manipulation
- Seaborn & Matplotlib — Visualization
- SciPy — Statistical analysis
- scikit-learn — Regression modeling

---

## Dataset
- **Source**: [Advertising Spend Dataset](http://bit.ly/ad_spend)
- Loaded via:
```python
URL_Ad_Spend = 'http://bit.ly/ad_spend'
Dataframe_Ad_Spend = pd.read_csv(URL_Ad_Spend)
```

---

## Objective
Predict sales based on advertising spend across TV, radio, and newspaper channels using linear regression.

---

## Methodology
1. **Load & Inspect Data**: `.shape`, `.info()`, `.head()`
2. **Data Cleaning & Transformations**: Adjust units for consistency
3. **Feature Engineering**: Create `total_ad_spend` and `roi_percent`
4. **Exploratory Analysis**:
   - Histogram of sales
   - Scatterplots and pairplots
   - Correlation matrix
5. **Modeling**:
   - Train/test split
   - Fit linear regression model
   - Evaluate performance (R²)

---

## Results Summary
- **TV and radio spend** show strong positive correlation with sales.
- Linear regression model explains a significant portion of variance (high R²).
- Predictions for new ad spend scenarios provided.

> **Conclusion**: TV and radio are key drivers of sales; newspaper has minimal impact.

---

## Visualizations
- Histogram of sales
- Scatterplot: TV spend vs. sales
- Pairplot of all ad channels
- Correlation heatmap

---

## How to Run
### Google Colab
Open: [Colab Notebook](https://colab.research.google.com/drive/1biipk8rwW8KrbrZhNZHAfXt8hH-7khL1)

### Local Environment
```bash
# Create virtual environment
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate

# Install dependencies
pip install pandas seaborn matplotlib scipy scikit-learn

# Run script
python gb881_assignment_6_schlichtmann_t.py
```

---

## Statistical Notes
- Correlation does not imply causation.
- Linear regression assumes linearity, independence, and homoscedasticity.

---

## Future Work
- Include **interaction terms** for combined ad effects.
- Explore **non-linear models** or **regularization techniques**.
- Add **cross-validation** for robust performance metrics.

---

## References
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Seaborn Documentation](https://seaborn.pydata.org/)
- [scikit-learn Linear Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html)

---

## 📄 License
MIT License — Educational use only.

