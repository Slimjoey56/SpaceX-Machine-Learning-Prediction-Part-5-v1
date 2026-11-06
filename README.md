# SpaceX Falcon 9 Landing Prediction

A supervised machine learning notebook comparing classification models for predicting first-stage booster landing outcomes.

This project was completed as part of the IBM Data Science Professional Certificate capstone learning pathway.

## Problem

Successful first-stage landings are relevant to reusable launch systems. This project examines whether historical launch characteristics can be used to classify landing outcomes.

## Models Compared

- Logistic Regression
- Support Vector Machine (SVM)
- Decision Tree Classifier
- K-Nearest Neighbors (KNN)

## Workflow

1. Prepare the modelling dataset.
2. Split observations into training and test sets.
3. Scale or transform features where required.
4. Train classification models.
5. Tune hyperparameters using GridSearchCV.
6. Compare model performance on the test set.

## Tools

- Python
- Pandas and NumPy
- scikit-learn
- Jupyter Notebook

## Repository Contents

```text
.
├── SpaceX-Machine-Learning-Prediction-Part-5-v1.ipynb
└── README.md
```

## Getting Started

Create an environment and install the pinned-minimum dependencies:

```bash
python -m venv .venv
# Windows PowerShell: .venv\\Scripts\\Activate.ps1
# macOS/Linux: source .venv/bin/activate
python -m pip install -r requirements.txt
jupyter notebook
```

The notebook downloads its modelling inputs directly from the IBM Skills Network-hosted CSV resources (`dataset_part_2.csv` and `dataset_part_3.csv`) using `pandas.read_csv` URLs embedded in the notebook. Those source files are not bundled in this repository; an internet connection is required when executing the data-loading cells. The notebook itself is the reproducible analysis entry point.

## Evaluation

The notebook describes accuracy-based comparison following hyperparameter tuning. Exact performance figures should be taken from the notebook output rather than inferred from this README.

For a stronger evaluation, document the test-set size, cross-validation strategy, confusion matrix, precision, recall, and F1-score. Ensure any fitted preprocessing steps are learned only from training data.

## Limitations

This is a course-based classification exercise, not a deployed prediction service. Model performance on a small historical dataset may not generalise to future launches.

## Related Projects

- [SpaceX Data EDA](https://github.com/Slimjoey56/spacex_launch_data_eda)
- [SpaceX Launch Site Analysis](https://github.com/Slimjoey56/SpaceX-Launch-Site-Location-Analysis)

## Author

Jehosaphat Brobbey Impiani  
[GitHub](https://github.com/Slimjoey56)