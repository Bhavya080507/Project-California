# California Housing Price Prediction

A Machine Learning project that predicts California house prices using Scikit-learn. The project includes data preprocessing, stratified train-test splitting, pipeline-based feature transformation, and a Random Forest Regression model.

## Features

- **Data Preprocessing:** Handles missing numerical values using median imputation and scales numerical features using StandardScaler.
- **Categorical Encoding:** Converts categorical features using OneHotEncoder.
- **Stratified Sampling:** Splits the dataset based on median income categories to maintain a representative distribution.
- **ML Pipeline:** Uses Scikit-learn's Pipeline and ColumnTransformer for consistent preprocessing.
- **Random Forest Regression:** Trains a model to predict median house values.
- **Inference:** Generates predictions for unseen housing data and exports results to CSV.

## Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Joblib

## Project Workflow

1. Load the California housing dataset.
2. Create income categories using `median_income` for stratified sampling.
3. Split the dataset into training and testing subsets.
4. Separate features and target values.
5. Build a preprocessing pipeline:
   - Median imputation
   - Standard scaling
   - One-hot encoding
6. Train a Random Forest Regressor.
7. Save the trained model and preprocessing pipeline using Joblib.
8. Use the saved pipeline and model to generate predictions on new data.

## How to Run

### 1. Clone the repository

```bash
git clone https://github.com/your-username/california-housing-prediction.git
cd california-housing-prediction
```

### 2. Install dependencies

```bash
pip install pandas numpy scikit-learn joblib
```

### 3. Run the project

```bash
python main.py
```

- On the first run, the model is trained and saved as `model.pkl` and `pipeline.pkl`.
- The test data is exported to `input.csv`.
- For inference, provide the input data in `new_input.csv` and rerun the script.
- Predictions are saved in `output.csv`.

## Model

The project uses `RandomForestRegressor` from Scikit-learn to predict `median_house_value` based on housing features.

# !!NO AI!!
Everything in this project is handwritten by human(my) hands.
