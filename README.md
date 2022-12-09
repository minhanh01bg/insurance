
<p>
  <br><br>
  <samp>
    I'm Minh Anh :wave:
  </samp>
</p>

# insurance
# Problem
Predict the price of insurance based on information about the insured person <br>
bài toán dự đoán giá tiền bảo hiểm dựa vào các thông tin về người bảo hiểm

# Data Description
Path: insurance.csv
<br><br>
The dataset contains the following fields:
- Year_last_admitted
- Weight_change_in_last_one_year
- age: age of primary beneficiary
- weight: self-reported weight of the insured person
- ...
- insurance: insurance price

# Data Cleaning

data has been preprocessed and cleaned

- Missing values <br>
Fill nan with mean value of the column <br>
- Outliers
-  Duplicated values
- ...

# Data normalization
- Text values are converted to numeric values with one hot encoding method<br>
- Values of each column are normalized to the range [0, 1] <br>
- Values of each column are normalized with the max value of the column

data cleaned and normalized is saved in cleaned_data.csv

# Build model linear regression

y_hat = w1 * x1 + w2 * x2 + ... + wn * xn + b <br>
Use loss function: MSE (mean squared error) <br>
- MSE = 1/n * sum(y - y_hat)^2 <br>
- y: real value <br>
- y_hat: predicted value <br>
- n: number of data <br>

derivative of MSE: <br>
- dMSE/dw = 1/n * sum(2 * (y - y_hat) * (-x)) <br>
- dMSE/db = 1/n * sum(2 * (y - y_hat) * (-1)) <br>

Model is built with gradient descent <br>
w = w - lr * gradient <br>
- lr: learning rate <br>
- gradient: gradient of loss function
- w: weight of model

⭐ From [Minh Anh](https://github.com/minhanh01bg)