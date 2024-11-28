
# Blood Glucose Prediction

<a target="_blank" href="https://cookiecutter-data-science.drivendata.org/">
    <img src="https://img.shields.io/badge/CCDS-Project%20template-328F97?logo=cookiecutter" />
</a>

## Overview

This project aims to predict blood glucose levels based on various physiological and dietary features using machine learning techniques. By processing and analyzing the data, the project seeks to provide valuable insights into glucose trends, enabling better management of diabetes and related conditions.

## Objectives
1. **Exploratory Data Analysis (EDA):** Uncover relationships and trends in the dataset.
2. **Feature Engineering:** Aggregate and preprocess features for improved predictive modeling.
3. **Predictive Modeling:** Train and evaluate machine learning models for accurate blood glucose level prediction.

## Key Features
- **Machine Learning Models:** Includes a trained linear regression model with plans for further algorithm exploration.
- **Comprehensive Preprocessing:** Handles missing values, scales features, and aggregates time-series data.
- **Visualization:** Correlation heatmaps and other plots to better understand feature relationships.

## Project Structure

```
├── LICENSE             <- Open-source license for project distribution.
├── Makefile            <- Commands for automating repetitive tasks like `make data` or `make train`.
├── README.md           <- Overview and documentation for developers and users.
├── data
│   ├── external        <- Data from third-party sources.
│   ├── interim         <- Intermediate data files during preprocessing.
│   ├── processed       <- Final cleaned and prepared datasets for modeling.
│   └── raw             <- Original data files before any transformations.
│
├── docs                <- Documentation and additional project details.
│
├── models              <- Trained models, serialized outputs, and predictions.
│
├── notebooks           <- Jupyter notebooks for analysis and experimentation.
│                         Example naming: `1.0-initial-data-exploration.ipynb`.
│
├── pyproject.toml      <- Metadata and configuration for project dependencies.
│
├── references          <- Manuals, research papers, and data dictionaries.
│
├── reports             <- Generated outputs like PDFs and visualizations.
│   └── figures         <- Graphs, plots, and images used in reporting.
│
├── requirements.txt    <- Python dependencies for environment setup.
│
├── setup.cfg           <- Configuration for code formatting and linting.
│
└── src                 <- Main project codebase.
    ├── __init__.py     <- Python module initialization.
    ├── config.py       <- Project-level configuration and constants.
    ├── dataset.py      <- Scripts for loading and processing datasets.
    ├── features.py     <- Feature engineering logic.
    ├── modeling/
    │   ├── __init__.py <- Modeling utilities.
    │   ├── predict.py  <- Inference scripts for predictions.
    │   └── train.py    <- Scripts for training machine learning models.
    └── plots.py        <- Functions to generate visualizations.
```

## Getting Started

### Prerequisites
- Python 3.8+
- Jupyter Notebook or a similar environment
- Required Python packages listed in `requirements.txt`

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/blood-glucose-prediction.git
   ```
2. Navigate to the project directory:
   ```bash
   cd blood-glucose-prediction
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Usage
1. **Run Data Preprocessing:**
   Use scripts in the `src/dataset.py` to clean and prepare data.
2. **Explore Data:**
   Open Jupyter notebooks in the `notebooks` directory for EDA.
3. **Train Models:**
   Use `src/modeling/train.py` to train machine learning models.
4. **Make Predictions:**
   Use `src/modeling/predict.py` for predictions using trained models.

## Results
The current linear regression model achieves:
- Mean Squared Error: 6.06
- R-squared: 0.33

Further improvements will focus on exploring advanced models like Random Forests or Neural Networks.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit changes and push to your fork.
4. Submit a pull request with details of your contribution.

## License
This project is licensed under the [MIT License](LICENSE).
