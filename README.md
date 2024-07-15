# Heart Disease Risk Clustering Project

This project aims to identify patients with a high risk of developing heart disease using unsupervised learning techniques. The analysis involves clustering patients based on their medical history and identifying risk factors associated with heart disease.

## Dataset

The heart disease dataset is obtained from the UCI Machine Learning Repository and contains 303 instances with 14 attributes, including age, sex, chest pain type, blood pressure, serum cholesterol, and a target variable indicating the presence or absence of heart disease.

## Steps Performed

### 1. Load the Dataset

The dataset was loaded into a pandas DataFrame and basic exploratory data analysis (EDA) was performed to understand its structure.

### 2. Exploratory Data Analysis (EDA)

EDA included basic statistics, checking for missing values, and visualizing the distribution of the target variable and other features.

### 3. Data Preprocessing

The dataset was preprocessed by handling missing values, scaling the features, and encoding categorical variables. The following steps were taken:
- Replaced missing values with the median value of each column.
- Scaled the numerical features using `StandardScaler`.

### 4. Clustering Algorithms Applied

Three clustering algorithms were applied to the preprocessed dataset:
- **K-means Clustering**
- **Hierarchical Clustering**
- **DBSCAN**

### 5. Dimensionality Reduction for Visualization

Principal Component Analysis (PCA) and t-SNE were used to reduce the dimensionality of the data and visualize the clusters formed by K-means.

### 6. Gaussian Mixture Models (GMMs)

GMMs were used to identify risk factors associated with heart disease and form clusters.

### 7. Evaluation of Clustering Performance

The clustering performance was evaluated using the following metrics:
- **Silhouette Score**: Measures how similar an object is to its own cluster compared to other clusters.
- **Davies-Bouldin Index**: Measures the average similarity ratio of each cluster with the one that is most similar to it.

## Results

Here are the results of the clustering algorithms:

- **Silhouette Score for K-means**: 0.13335696483847778
- **Silhouette Score for Hierarchical**: 0.11511622103926623
- **Davies-Bouldin Index for K-means**: 2.1222923727015943
- **Davies-Bouldin Index for Hierarchical**: 2.168177899907483
- **Davies-Bouldin Index for GMM**: 2.3601840229795177

### Interpretation

- The silhouette scores are relatively low, suggesting that the clusters are not well-defined.
- The Davies-Bouldin indices are relatively high, indicating that the clusters are not well separated.


## Dependencies

- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

## How to Run

1. Clone this repository.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Run the Jupyter Notebook or Python script to load the dataset, preprocess the data, apply clustering algorithms, and evaluate the results.

## License

This project is licensed under the MIT License.

## Acknowledgements

The dataset used in this project is from the UCI Machine Learning Repository.

