## 🚗 Car Prices

### 🎯 Objective
- Prepare the dataset for modeling
- Apply feature selection to identify the most informative variables
- Classify cars as **cheap** or **expensive**

### 🧹 Data Cleaning
- Removed **14 duplicate rows**
- Handled missing values:
  - `carwidth` → mean imputation (after replacing `*` with NaN)
  - `enginelocation` → most frequent value

### 📏 Feature Scaling
- `carwidth`, `stroke`, `peakrpm` → RobustScaler
- `curbweight` → StandardScaler
- `cylindernumber` → mapped to numeric values and scaled

### 🔤 Feature Encoding
- `aspiration`, `enginelocation` → One-Hot Encoding (binary)
- `enginetype` → One-Hot Encoding (multi-class)
- `price` → Label Encoding (`0 = cheap`, `1 = expensive`)

### 🤖 Base Model
- Model: Logistic Regression
- Evaluation: Cross-Validation
- Base model accuracy: **~0.88**

### 🔍 Feature Selection
- Method: Permutation Importance
- Weak features removed (importance ≤ 0.05)
- Strong features identified:
  - `carwidth`
  - `curbweight`

### 📈 Final Model Performance
- Accuracy before feature selection: **~0.85**
- Accuracy after feature selection: **~0.90**

### ⚖️ Stratification
- Used stratified splitting to preserve class distribution
- Applied `stratify=y` in train-test split
- Demonstrated stratification with `StratifiedKFold`
