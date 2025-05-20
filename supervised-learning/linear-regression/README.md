# Linear Regression: An Introduction

Linear Regression is one of the most fundamental algorithms in machine learning and statistics. It models the relationship between a **dependent variable** (target) and one or more **independent variables** (features) by fitting a **linear equation** to the observed data.

The simple linear regression equation is:  
$y = \theta_0 + \theta_1 x + \varepsilon$

Where:
- `y` is the predicted value (target)
- `x` is the input feature
- `θ₀` is the intercept (bias)
- `θ₁` is the coefficient (slope)
- `ε` is the error term

## Why is Linear Regression Important?

Linear regression is important because:
- It’s **interpretable** — you can clearly see how input features affect the output.
- It’s **efficient** — easy to compute and fast to train.
- It forms the **foundation** for many advanced algorithms.
- It provides insights into data relationships through coefficients.
- It helps in **predictive modeling** where the relationship between variables is linear.

## Real-World Applications of Linear Regression

### 1. **Business Forecasting**
Companies use linear regression to predict future sales based on advertising spend, seasonal patterns, or economic indicators.

### 2. **Healthcare**
Helps in predicting patient outcomes, such as estimating blood pressure based on age, weight, and other variables.

### 3. **Real Estate**
Used to estimate property prices based on features like area, location, number of bedrooms, etc.

### 4. **Finance**
Models relationships between economic indicators (e.g., predicting stock prices based on trading volume or market indices).

### 5. **Marketing Analytics**
Analyzes the impact of marketing campaigns on sales or customer behavior, helping optimize advertising strategies.

---
### 📉 Evaluation Metrics for Regression

### Mean Absolute Error (MAE)
The MAE measures the average absolute difference between predicted and actual values:

$$
\text{MAE} = \frac{1}{n} \sum_{i=1}^{n} \left| y_i - \hat{y}_i \right|
$$

### Mean Squared Error (MSE)
The MSE measures the average squared difference between predicted and actual values:

$$
\text{MSE} = \frac{1}{n} \sum_{i=1}^{n} \left( y_i - \hat{y}_i \right)^2
$$

### Root Mean Squared Error (RMSE)
The RMSE is the square root of MSE, giving an error metric in the same units as the target:

$$
\text{RMSE} = \sqrt{ \frac{1}{n} \sum_{i=1}^{n} \left( y_i - \hat{y}_i \right)^2 }
$$

### Coefficient of Determination (R² Score)

The R² score (coefficient of determination) measures how well the regression model explains the variance in the target variable. It is defined as:

<img width="314" alt="Screenshot 2025-05-19 at 6 22 35 PM" src="https://github.com/user-attachments/assets/835901d4-fccd-444d-869d-695fe05c2afe" />

An \( R^2 \) score close to 1 indicates that the model explains a large portion of the variance in the data.

---
Linear regression remains a cornerstone in both academic research and industry due to its simplicity, efficiency, and wide applicability in solving real-world problems.

