<h1 align="center">Data Science & Machine Learning : Crypto Target Prediction Project<p align="center"></h1>

<h1 align="center">Bar Bettash<p align="center">
<a href="https://www.linkedin.com/in/barbettash/" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="LinkedIn" height="30" width="40" /></a>
</h1>


<!-- ABOUT THE PROJECT -->

The project performs feature engineering, visualization, and model training using logistic regression to predict the 'target' (price increase/decrease).

### Data from
(https://www.kaggle.com/competitions/directional-forecasting-in-cryptocurrencies/overview)

### Built With

Python <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a>

![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) <a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/pandas/pandas-original.svg" alt="pandas" width="40" height="40"/> </a>

![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)  <a href="https://numpy.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/numpy/numpy-original.svg" alt="numpy" width="40" height="40"/> </a>

![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) <a href="https://matplotlib.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/matplotlib/matplotlib-original.svg" alt="matplotlib" width="40" height="40"/> </a>

![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white) </p>


<!-- GETTING STARTED -->
## Getting Started


### Prerequisites

To run the project, you need the following libraries installed:

* pandas: A powerful library for data manipulation, analysis, and loading data from various sources (CSV in this case).
  ```sh
  pip install pandas

* numpy: Provides efficient operations on numerical data (arrays, matrices) essential for machine learning algorithms.
  ```sh
  pip install numpy

* matplotlib: Used for creating static visualizations like histograms and scatterplots to explore data.
  ```sh
  pip install matplotlib

* seaborn: A high-level library built on top of matplotlib for creating more sophisticated and visually appealing data visualizations.
  ```sh
  pip install seaborn

* scikit-learn: For machine learning algorithms. Offers functions for splitting datasets into training and testing sets, a crucial step in machine learning.
  ```sh
  pip install scikit-learn

* joblib: For saving and loading machine learning models.
  ```sh
  pip install joblib

### Load dataset:

Google Drive Setup: The script mounts Google Drive to access CSV files containing cryptocurrency data. It loads these files into a dictionary of DataFrames.

## Feature Engineering:

A class FeatureEngineering is implemented to create additional features:

* Price change (price_change) based on the percentage difference between the open and close prices.

* Volatility calculated as a percentage of the closing price.

* Exponential moving averages (EMA) for 5, 12, and 26 periods.

* MACD (Moving Average Convergence Divergence) and signal line based on EMAs.

* Lagged features for volume and close prices.

* The target variable is converted into a categorical feature, and NaN rows are dropped.

### Bar Plot: 

For the distribution of the target variable.

### Correlation heatmap: 

Shows the relationships between features, with notable observations such as high correlations between price features and weak correlations between the target and most features.

![image](https://github.com/user-attachments/assets/37cbb255-d703-4365-ae84-1f642a254ada)


### Scatterplot: 

for the relationship between volume and price change, noting a lack of strong linear correlation.

![image](https://github.com/user-attachments/assets/3743f800-c9cd-4bfb-91d4-ce492fc779a2)

## Model Training:

### Train-test split: 

The dataset is split into training and testing sets, and the features are scaled using StandardScaler.

### Logistic regression: 

Applied to classify whether the price will go up or down (target).

### Model evaluation: 
After training, model performance is evaluated using accuracy, classification report, and confusion matrix.

## Scaling and Model Optimization:

### Scaling: 
The model and scaler are saved and reloaded using joblib.

### Example:
--------------------------------------------------

The model's F1 accuracy is 0.53

--------------------------------------------------

<!-- CONTACT -->
## Contact

<p align="left">
<a href="https://www.linkedin.com/in/barbettash/" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="https://www.linkedin.com/in/barbettash/" height="30" width="40" /></a>
</p>


**bar.bettash.jobs@gmail.com** 


<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

This code is provided "as is" and may not function as intended in the future due to potential updates to external libraries, frameworks, websites, or APIs it interacts with. The code is no longer actively maintained and may require modifications to adapt to future changes.

**Recommendations:**

* Keep an eye on updates to libraries and dependencies to ensure compatibility.
* Be prepared to adapt the code based on future changes in the target website or API.








  
