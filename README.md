GLD Price Prediction using ML algorithms
This project predicts the GLD (Gold) prices using ML algorithms. It reads a dataset of various financial indicators, processes the data, and compares actual versus predicted GLD prices, visualizing the results using a bar graph.

Dataset
The dataset (gld_price_data.csv) contains historical data related to the price of Gold (GLD) and other financial indicators, such as:

USO (United States Oil Fund)
SPX (S&P 500 Index)
SLV (Silver ETF Price)
EUR/USD (Euro to USD exchange rate)
GLD (Gold Price)
The file is expected to be a CSV file with the following columns:

Date: The date for each entry (will be dropped in preprocessing)
USO, SPX, SLV, EUR/USD, and GLD: Numerical values representing different financial indicators.
Prerequisites
Before running the code, ensure you have the following Python packages installed:

pandas
numpy
scikit-learn
matplotlib
You can install these dependencies using pip:

bash
Copy code
pip install pandas numpy scikit-learn matplotlib
Code Overview
Importing Libraries:

The code imports necessary libraries including pandas for data manipulation, numpy for numerical operations, SVC from sklearn for building the SVM model, and matplotlib for visualization.
Reading and Processing the Data:

The dataset is read from the CSV file, and unnecessary columns (Date) are removed.
Numerical columns are cast to integer types for consistency in the modeling process.
Splitting Data:

The feature variables (X) are selected as the financial indicators excluding GLD, while the target variable (y) is the GLD column.
The dataset is split into training (80%) and testing (20%) sets using train_test_split().
Training the SVM Model:

The model is trained using the ML ALGORITHMS.
The model is trained on the training data (X_train, y_train), and predictions are made on the testing data (X_test).
Evaluation:

The code computes a confusion matrix and R² score to evaluate the model’s performance.
The R² score is printed, which indicates how well the model fits the data.
Visualization:

A bar graph is plotted to compare the actual and predicted values of GLD prices for each test data point.
The graph includes side-by-side bars representing actual and predicted GLD prices, making it easy to see where the model’s predictions diverge from the actual values.
