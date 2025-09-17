# RPUF: Predicted AD TC and CS

It was used to predict the apparent density (AD), thermal conductivity (TC) and compressive strength (CS) of rigid polyurethane foam (RPUF)

### Main Features

Main Features
<ul>
  <li>★ Feature engineering (calculating foam gas production, etc.)</li>
  <li>★ Regression and classification models for performance prediction and type differentiation</li>
  <li>★ SHAP analysis and correlation analysis</li>
  <li>★ Streamlit visualization interface</li>
</ul>

## Installation

1. Clone the repository:
```bash
git clone https://github.com/big-material/DQ.git
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
If there is no requirements.txt, please manually install pandas, numpy, scipy, scikit-learn, streamlit, joblib, dcor, etc.

## Usage

### 1. Use as a library
```python
from DQ.DCC import dcc, dcc_feature
from DQ.Correlation import pearson_matrix, spearman_matrix
import pandas as pd

df = pd.read_csv('your_data.csv')
result = dcc(df, ratio=0.1)
```

### 2. Launch Streamlit visualization interface
```bash
streamlit run runner.py
```

### 3. Main APIs
- `dcc(data, ratio, eps, corr_func)`: Analyze the impact of missing data ratio on correlation coefficients

For more usage, please refer to the source code and comments.

# Reference

Evaluate dataset quality using correlation convergency inspired from perturbation theory. submit.

