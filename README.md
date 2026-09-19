# Agricultural Crop Yield Prediction Using Artificial Neural Networks (ANN)

A deep learning regression project that predicts agricultural crop yield using environmental, soil, crop, and farming-related features. The project applies exploratory data analysis (EDA), data preprocessing, and Artificial Neural Networks (ANN).

## Highlights

- Exploratory data analysis of agricultural features
- Missing value imputation for numerical and categorical data
- One-hot encoding and feature scaling using StandardScaler
- Baseline and improved ANN model experiments
- Dropout, early stopping, and learning rate scheduling
- Model evaluation using MAE, RMSE, and R²

## Data

The dataset contains **500 records and 22 columns**, including:
- Region and crop type
- Soil and environmental features
- Irrigation and farming information
- Crop disease status and NDVI index
- Crop yield as the target variable

## Model Experiments

Two ANN architectures were explored:
- Baseline ANN: Two dense layers with ReLU activation and a linear output layer.
- Improved ANN: Simplified architecture with dropout, early stopping, and learning rate scheduling to reduce overfitting.

## Results

The improved model achieved lower MAE and RMSE. However, both models produced negative R² values, indicating that the model performance remained limited by the available features and dataset.

## How to Run

The notebook was developed using Python and Jupyter Notebook.

1. Clone this repository:

```
git clone https://github.com/your-username/agricultural-crop-yield-prediction.git
```

2. Install the required libraries:

```
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow pyarrow jupyter
```

3. Ensure the dataset is located at: `data/agricultural_crop_yield.parquet`
4. Open the notebook: `notebook/Agricultural Crop Yield Prediction Using ANN.ipynb`
5. Run all cells to perform data preprocessing, exploratory data analysis, model training, and evaluation.
