# K-Means Clustering on Wholesale Customers Dataset

## Objective
Perform **unsupervised learning** using **K-Means clustering** to identify customer segments in the Wholesale Customers dataset.

---

## Tools & Libraries
- Python 3.x
- `pandas`
- `scikit-learn`
- `matplotlib`
- `seaborn`

---

## Dataset Information

- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers)
- **Features**:
  - `Fresh`, `Milk`, `Grocery`, `Frozen`, `Detergents_Paper`, `Delicassen`
- **Shape**: 440 rows × 8 columns (including `Channel` and `Region`)

---

## Steps Performed

### 1. Load and Explore the Data
- Loaded the dataset from UCI.
- Dropped non-numeric categorical features (`Channel`, `Region`) to focus on spending behavior.

### 2. Data Preprocessing
- Standardized the features using `StandardScaler` for effective distance-based clustering.

### 3. Elbow Method
- Applied K-Means clustering for values of **K = 1 to 10**.
- Plotted the **Elbow Curve** to identify the optimal number of clusters.

### 4. Clustering with K-Means
- Selected **K = 3** (based on elbow curve).
- Fit the KMeans model and assigned cluster labels to each customer.

### 5. Visualization
- Applied **PCA (Principal Component Analysis)** to reduce data to 2 dimensions.
- Visualized clusters in a 2D scatter plot with distinct colors.

### 6. Evaluation
- Used **Silhouette Score** to evaluate clustering performance.


## Results

- **Optimal Clusters**: 3
- **Silhouette Score**: ~0.29 (indicates moderate cluster separation)
- Visualizations show distinct clusters in PCA-reduced space.

