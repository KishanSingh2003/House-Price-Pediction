# House Price Prediction

A machine learning project designed to predict house prices based on various real estate features. The project leverages advanced regression models such as CatBoost, enabling accurate price predictions for buyers, sellers, and real estate professionals.

---

## Table of Contents
- [About The Project](#about-the-project)
- [Getting Started](#getting-started)
  - [Dependencies](#dependencies)
  - [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Data Sources](#data-sources)
- [Results](#results)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Authors & Acknowledgements](#authors--acknowledgements)

---

## About The Project

This project aims to accurately predict house prices using a range of relevant features such as location, size, and condition. Through exploratory data analysis, rigorous cleaning, and the use of powerful regression algorithms (especially CatBoost with hyperparameter tuning), the project produces valuable outputs including trained models, evaluation metrics, and visualizations. This solution empowers data-driven real estate valuation and decision-making.

**Technologies used:**  
Python, Jupyter notebooks, Pandas, NumPy, Scikit-learn, CatBoost

**Main datasets:**  
HousePricePrediction.xlsx - clean and formatted housing data  
strat_train_set.csv, strat_test_set.csv - stratified data splits for training and validation

---

## Getting Started

### Dependencies

To run this project, make sure you have these core packages installed:

Or, use the provided environment file:

### Installation

1. Clone this repository:
2. Install dependencies:

---

## Usage

- Open and follow the steps in `.EDA_And_DataCleaning.ipynb` to explore, clean, and prepare the dataset.
- Train and evaluate models using `Training_Models.ipynb`. You can change parameters and view results.
- Results and metrics will be saved in the `catboost_info` folder:
- `catboost_training.json` holds CatBoost training details.
- `learn_error.tsv` logs training errors/losses.
- `time_left.tsv` logs remaining training time.
- `learn/events.out.tfevents` contains logs for further inspection (TensorBoard, etc.).
- CSV and Excel files hold input data and splits:
- `HousePricePrediction.xlsx`
- `strat_train_set.csv`, `strat_test_set.csv`

---

## Project Structure

<pre>
HousePricePrediction/
├── catboost_info/
│   ├── catboost_training.json
│   ├── learn_error.tsv
│   ├── time_left.tsv
│   └── learn/
│       └── events.out.tfevents
├── .EDA_And_DataCleaning.ipynb
├── HousePricePrediction.xlsx
├── Training_Models.ipynb
├── strat_test_set.csv
├── strat_train_set.csv
├── LICENSE
└── README.md
</pre>


---

## Data Sources

- **HousePricePrediction.xlsx** - The main dataset with housing features and prices.
- **strat_train_set.csv** / **strat_test_set.csv** - Train and test splits created from the main dataset for validation.

---

## Results

- Trained CatBoost models with hyperparameter tuning.
- Prediction metrics and error logs saved in the `catboost_info` folder.
- Jupyter notebooks visualize feature analysis and prediction results.
- The CatBoost regressor was trained and evaluated on the dataset. Model performance is as follows:

| Metric             |   Train       |   Test       |
|:------------------:|:------------:|:------------:|
| RMSE (Error)       | 18,225.08    | 36,185.77    |
| R²                 | 0.9443       | 0.8293       |



These results indicate strong predictive power on the training set and good generalization to the test set.

---

## Roadmap

- Improve preprocessing and feature engineering.
- Try additional regression algorithms.
- Add deployment scripts for model serving.
- Expand to more regions/datasets.

---

## Contributing

Pull requests are welcome!  
For major changes, please open an issue first to discuss what you'd like to change.

---

## License

Distributed under the MIT License. See LICENSE for details.

---

## Authors & Acknowledgements

Author: Kishan Kumar Singh

Thanks to all collaborators, contributors, and open-source communities for tools and inspiration.

