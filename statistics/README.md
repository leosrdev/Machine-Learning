## Normal (Gaussian) Distribution

The Gaussian distribution, also known as the Normal distribution or bell curve, is a continuous probability distribution that is symmetric around its mean.

### 1. One-Dimensional Gaussian Distribution

A **one-dimensional (univariate) normal distribution** describes a continuous random variable whose values cluster around a central mean, with the spread controlled by the variance.

<img width="744" height="513" alt="image" src="https://github.com/user-attachments/assets/52fec8e9-ee76-4689-99fe-f70822e8dce1" />



**Probability Density Function (PDF)**

The 1D normal distribution is defined as:

$$
f(x) = \frac{1}{\sqrt{2\pi \sigma^2}} \exp\left( -\frac{(x - \mu)^2}{2\sigma^2} \right)
$$

**Mean (μ)**

The mean represents the central value of the distribution:

$$
\mu = \frac{1}{N} \sum_{i=1}^{N} x_i
$$

**Variance (σ²)**

Variance measures how spread out the values are:

$$
\sigma^2 = \frac{1}{N} \sum_{i=1}^{N} (x_i - \mu)^2
$$

---

### 2. Two-Dimensional Gaussian Distribution

A **two-dimensional (bivariate) Gaussian distribution** models data with two correlated variables. Instead of a bell curve, the distribution forms a **bell-shaped surface** or **elliptical contours**.

<img width="448" height="369" alt="image" src="https://github.com/user-attachments/assets/87cd869b-a02a-4c18-9b65-a609c54687c3" />


**Probability Density Function (PDF)**

The 2D Gaussian is defined as:

$$
f(\mathbf{x}) = \frac{1}{2\pi\sqrt{|\Sigma|}} \exp \left( -\frac{1}{2} (\mathbf{x} - \boldsymbol{\mu})^T \Sigma^{-1} (\mathbf{x} - \boldsymbol{\mu}) \right)
$$

Where:

* $\mathbf{x} = [x_1, x_2]^T$
* $\boldsymbol{\mu} = [\mu_1, \mu_2]^T$ is the mean vector
* $\Sigma$ is the covariance matrix

**Mean Vector**

$$
\boldsymbol{\mu} = \begin{bmatrix}
\mu_1 \
\mu_2
\end{bmatrix}
$$

**Covariance formula**

$$\text{Cov}(X, Y) = s_{xy} = \frac{1}{N-1} \sum_{i=1}^{N} (x_i - \bar{x})(y_i - \bar{y})$$


**Covariance Matrix (x,y variables)**

$$
\begin{pmatrix}
var(x) & cov(x,y) \\
cov(x,y) & var(x)
\end{pmatrix}
$$






