# Gaussian (Normal) Distribution

This README introduces the **Gaussian (Normal) Distribution)** in both one and two dimensions. It explains key concepts such as the **mean**, **variance**, and **covariance**, and provides visual placeholders where charts can be inserted.

---

## 1. One-Dimensional Gaussian Distribution

A **one-dimensional (univariate) normal distribution** describes a continuous random variable whose values cluster around a central mean, with the spread controlled by the variance.

### **Probability Density Function (PDF)**

The 1D normal distribution is defined as:

$$
f(x) = \frac{1}{\sqrt{2\pi \sigma^2}} \exp\left( -\frac{(x - \mu)^2}{2\sigma^2} \right)
$$

### **Mean (μ)**

The mean represents the central value of the distribution:

$$
\mu = \frac{1}{N} \sum_{i=1}^{N} x_i
$$

### **Variance (σ²)**

Variance measures how spread out the values are:

$$
\sigma^2 = \frac{1}{N} \sum_{i=1}^{N} (x_i - \mu)^2
$$

### **Chart Placeholder**

*(You can insert a 1D Gaussian curve image here)*

---

## 2. Two-Dimensional Gaussian Distribution

A **two-dimensional (bivariate) Gaussian distribution** models data with two correlated variables. Instead of a bell curve, the distribution forms a **bell-shaped surface** or **elliptical contours**.

### **Probability Density Function (PDF)**

The 2D Gaussian is defined as:

$$
f(\mathbf{x}) = \frac{1}{2\pi\sqrt{|\Sigma|}} \exp \left( -\frac{1}{2} (\mathbf{x} - \boldsymbol{\mu})^T \Sigma^{-1} (\mathbf{x} - \boldsymbol{\mu}) \right)
$$

Where:

* $\mathbf{x} = [x_1, x_2]^T$
* $\boldsymbol{\mu} = [\mu_1, \mu_2]^T$ is the mean vector
* $\Sigma$ is the covariance matrix

### **Mean Vector**

$$
\boldsymbol{\mu} = \begin{bmatrix}
\mu_1 \
\mu_2
\end{bmatrix}
$$

### **Covariance Matrix**

$$
\Sigma = \begin{bmatrix}
\sigma_1^2 & \sigma_{12} \
\sigma_{12} & \sigma_2^2
\end{bmatrix}
$$

Where:

* $\sigma_1^2$ and $\sigma_2^2$ are the variances of the two variables
* $\sigma_{12}$ is the covariance between the two variables

### **Chart Placeholder**

*(You can insert a 2D contour or surface plot here)*

---

## 3. Example Application — Modeling Human Height

A classic real-world application of the normal distribution is **modeling human height**.

If you collect height measurements from **20 people**, the distribution of these heights will often approximate a Gaussian curve.

### Steps in the analysis:

1. **Collect height data** (e.g., 20 values in centimeters).
2. Compute the **mean** height:
   $$ \mu = \frac{1}{20} \sum_{i=1}^{20} h_i $$
3. Compute the **variance**:
   $$ \sigma^2 = \frac{1}{20} \sum_{i=1}^{20} (h_i - \mu)^2 $$
4. Plot a **histogram** of the values.
5. Overlay the **Gaussian curve** using the computed parameters.

This demonstrates how Gaussian distributions naturally arise in biological measurements due to many small contributing factors.

---

Feel free to insert charts where indicated to complete the visualization!
