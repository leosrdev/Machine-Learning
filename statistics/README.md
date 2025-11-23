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

### 3. Application of normal distribuition
In this example we will calculate the probability of finding a NBA player with height between 200 and 210 cm given a normal distribuition of heights.


**NBA Players**

| Player              | Height (cm) |
|---------------------|-------------|
| LeBron James        | 203         |
| Michael Jordan      | 198         |
| Shaquille O’Neal    | 216         |
| Stephen Curry       | 188         |
| Kobe Bryant         | 198         |
| Kevin Durant        | 206         |
| Magic Johnson       | 206         |
| Tim Duncan          | 211         |
| Yao Ming            | 229         |
| Kareem Abdul-Jabbar | 218         |


The mean:

$$
\mu = \frac{1}{N} \sum_{i=1}^{N} x_i = \frac{203+198+216+188+198+206+206+211+229+218}{10} = 207.3cm
$$

The variance:

$$
\begin{matrix}
(203-207.3)^2+ \\  
(198-207.3)^2+ \\
(216-207.3)^2+ \\ 
(188-207.3)^2+ \\ 
(198-207.3)^2+ \\ 
(206-207.3)^2+ \\ 
(206-207.3)^2+ \\ 
(211-207.3)^2+ \\ 
(229-207.3)^2+ \\ 
(218-207.3)^2  
\end{matrix}
$$

$$
\sum_{i=1}^{N} (x_i - \mu)^2 = 1240.9
$$


$$
\sigma^2 = \frac{1}{N} \sum_{i=1}^{N} (x_i - \mu)^2 = \frac{1240.9}{10} = 124.09 (cm^2)
$$

The standard deviation:

$$
\sigma = \sqrt{\sigma^2} = 11.14 cm
$$

Convert heights to Z scores  
For 200 cm  

$$
z_1 = \frac{x_1 - \mu}{\sigma} = \frac{200-207.3}{11.14} = -0.655
$$

$$
z_2 = \frac{x_2 - \mu}{\sigma} = \frac{210-207.3}{11.14} = 0.242
$$

From starndard normal [CDF](https://en.wikipedia.org/wiki/Standard_normal_table) tables:  

$$
\Phi(z_1) \approx 0.256, \quad \Phi(z_2) \approx 0.596
$$

$$
P(200 < X < 210) \approx 0.596 - 0.256
$$

$$
P(200 < X < 210) \approx 0.340
$$

This means there is a 34% probability that a randomly chosen player has a height between 200 cm and 210 cm.
