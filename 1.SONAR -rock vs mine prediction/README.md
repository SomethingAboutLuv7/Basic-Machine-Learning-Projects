# Sonar - Rock vs Mine Prediction

A binary classification project that predicts whether a detected underwater object is a **Rock (`R`)** or a **Mine (`M`)** based on sonar signals bounced off cylinders at various angles.

## Dataset
- **File**: `sonarmine.csv`
- **Features**: 60 numerical attributes representing the energy within a particular frequency band, integrated over a certain period of time.
- **Target**: Label column indicating:
  - `R`: Rock
  - `M`: Mine

## Workflow
1. **Data Loading & Exploration**: Read sonar chirp data with `pandas` and inspect statistical distributions.
2. **Preprocessing**: Label separation and feature normalization/indexing.
3. **Train-Test Split**: Partitioning data into training and test sets using `train_test_split` with stratification.
4. **Model Training**: Fitting a `LogisticRegression` model on the training data.
5. **Evaluation**: Assessing model accuracy on both training and test data.
6. **Predictive System**: Testing on single input instances to classify new sonar frequency readings.

## Requirements
```bash
pip install numpy pandas matplotlib scikit-learn jupyter
```

## Running the Notebook
Open and run the notebook:
```bash
jupyter notebook rockmine.ipynb
```
