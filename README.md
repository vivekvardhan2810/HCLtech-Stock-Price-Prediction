# HCLtech Stock Price Prediction

This project performs stock price prediction for HCLtech using three machine learning models: Linear Regression, Support Vector Machines (SVM), and K-Means Clustering. The project includes data preprocessing, Exploratory Data Analysis (EDA), model training, evaluation, and stock price analysis.

## Table of Contents
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Models Used](#models-used)
  - [Linear Regression](#linear-regression)
  - [Support Vector Machines (SVM)](#support-vector-machines-svm)
  - [K-Means Clustering](#k-means-clustering)
- [Evaluation](#evaluation)
- [Contributing](#contributing)
- [License](#license)

## Dataset

The dataset used for this project contains historical stock prices for HCLtech, including columns like `Date`, `Open`, `High`, `Low`, `Close`, and `Volume`.

**Columns in the dataset:**

- `Date`: Date of the stock data
- `Open`: Opening price of the stock
- `High`: Highest price of the stock on that day
- `Low`: Lowest price of the stock on that day
- `Close`: Closing price of the stock
- `Volume`: Number of shares traded on that day

## Installation

To run this project, follow the steps below:

1. Clone the repository:

   ```
   git clone https://github.com/your-username/hcltech-stock-prediction.git
   cd hcltech-stock-prediction
   ```

2. Install the required dependencies:

   ```
   pip install -r requirements.txt
   ```

3. Place the ```HCLTECH.csv``` dataset in the project directory.

## Usage

After installing the dependencies and placing the dataset in the directory, you can run the project using the following command:

```
python stock_prediction.py
```

This will perform EDA, data preprocessing, and train the models, generating evaluation metrics for each model. It will also display stock price charts and cluster visualizations.

## Models Used

## Linear Regression

Linear Regression is a simple model that assumes a linear relationship between the input features (```Open```, ```High```, ```Low```, ```Volume```) and the target variable (```Close price```). It fits a line to predict future stock prices.

**Steps**:

- Data Preprocessing

- Splitting the dataset into training and testing sets

- Training the Linear Regression model

- Evaluating the model using Mean Squared Error (MSE) and R² score

## Support Vector Machines (SVM)

SVM is a powerful regression model that uses kernels to map the input data into higher dimensions and find optimal boundaries. In this project, we use an RBF kernel to predict stock prices.

**Steps**:

- Scaling the data using ```StandardScaler```

- Training the SVM model

- Predicting stock prices

- Evaluating the model with MSE and R² score

## K-Means Clustering

K-Means Clustering is an unsupervised learning algorithm used to group data points into clusters. We apply it to group the stock price trends into clusters.

**Steps**:

- Using the ```Close``` price for clustering

- Visualizing the clusters

## Evaluation

Each model is evaluated based on:

- **Mean Squared Error (MSE)**: Measures the average squared difference between actual and predicted values.

- **R² Score**: Represents the proportion of variance explained by the model.

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue for improvements or suggestions.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
