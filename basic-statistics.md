## Measures of Central Tendency

Measures of central tendency are statistical measures used to describe the center or typical value of a dataset. They provide a single value around which the data tends to cluster. There are several measures of central tendency, including moments, skewness, and kurtosis. Each of these measures provides different insights into the distribution of data and helps in understanding its characteristics. Let's explore each of them:

### Moments

Moments are numerical values that summarize the shape and distribution of a dataset. The term "moment" comes from mathematical physics and is used in statistics to characterize the distribution of data points around the mean. There are several types of moments, but the first four moments are the most commonly used:

- $\textbf{First Moment (Mean):}$  The first moment is the arithmetic mean of a dataset and is denoted by $\mu$ . It represents the center of mass or average value of the data points.

Mathematically, the mean $\mu$ of a dataset with $n$ data points $\{x_1, x_2, ..., x_n\}$ is calculated as:

$$
\begin{equation*}
\mu = \frac{1}{n} \sum_{i=1}^{n}x_i
\end{equation*}
$$
For a continuous random variable $X$ with probability density function $f(x)$, the first moment about the origin (mean) is given by:

$$
\mu = \int{x \cdot f(x) \, dx} \quad \text{from} \, -\infty \, \text{to} \, +\infty
$$
- $\textbf{Second Moment (Variance):}$ The second moment measures the spread or dispersion of the data points around the mean. It is denoted by $\sigma^2$ (sigma squared) and is the average of the squared differences between each data point and the mean.

Mathematically, the variance $\sigma^2$ of a dataset with $n$ data points $\{x_1, x_2, ..., x_n\}$ and mean $\mu$ is calculated as:

$$
\begin{equation*}
\sigma^2 = \frac{1}{n} \sum_{i=1}^{n}(x_i-\mu)^2
\end{equation*}
$$
For a continuous random variable $X$ with probability density function $f(x)$, the second moment about the origin (variance) is given by:

$$
\sigma^2 = \int{(x - \mu)^2 \cdot f(x) \, dx} \quad \text{from} \, -\infty \, \text{to} \, +\infty
$$
- $\textbf{Third Moment (Skewness):}$ Skewness measures the asymmetry of the data distribution. It indicates whether the data is skewed to the left (negative skewness) or to the right (positive skewness) compared to the mean. Skewness is denoted by $\gamma_1$ (gamma one).

Mathematically, the skewness $\gamma_1$ of a dataset with $n$ data points $\{x_1, x_2, ..., x_n\}$ and mean $\mu$ is calculated as:

$$
\begin{equation*}
\gamma_1 = \frac{\frac{1}{n}\sum_{i=1}^{n}(x_i-\mu)^3}{\left(\frac{1}{n}\sum_{i=1}^{n}(x_i-\mu)^2\right)^{\frac{3}{2}}}
\end{equation*}
$$
For a continuous random variable $X$ with probability density function $f(x)$, the third central moment (related to skewness) is given by:

$$
\gamma_3 = \int{(x - \mu)^3 \cdot f(x) \, dx} \quad \text{from} \, -\infty \, \text{to} \, +\infty
$$
- $\textbf{Fourth Moment (Kurtosis):}$ Kurtosis measures the shape of the distribution and assesses the presence of outliers or heavy tails. High kurtosis indicates a sharper peak and heavier tails, while low kurtosis indicates a flatter peak and lighter tails. Kurtosis is denoted by $\gamma_2$ (gamma two).

Mathematically, the kurtosis $\gamma_2$ of a dataset with $n$ data points $\{x_1, x_2, ..., x_n\}$ and mean $\mu$ is calculated as:

$$
\begin{equation*}
\gamma_2 = \frac{\frac{1}{n}\sum_{i=1}^{n}(x_i-\mu)^4}{\left(\frac{1}{n}\sum_{i=1}^{n}(x_i-\mu)^2\right)^2}
\end{equation*}
$$
For a continuous random variable $X$ with probability density function $f(x)$, the fourth central moment (related to kurtosis) is given by:

$$
\gamma_4 = \int{(x - \mu)^4 \cdot f(x) \, dx} \quad \text{from} \, -\infty \, \text{to} \, +\infty
$$

### Skewness

Skewness is a measure of the asymmetry of a probability distribution. It quantifies the extent to which a dataset deviates from being symmetrical. The skewness value can be positive, negative, or zero:

- $\textbf{Positive Skewness:}$ A positive skewness value indicates that the data is skewed to the right, meaning the tail on the right side of the distribution is longer, and the majority of the data points are concentrated on the left side.
- $\textbf{Negative Skewness:}$ A negative skewness value indicates that the data is skewed to the left, meaning the tail on the left side of the distribution is longer, and the majority of the data points are concentrated on the right side.
- $\textbf{Zero Skewness:}$ A skewness value close to zero suggests that the data is approximately symmetrically distributed.

### Kurtosis

Kurtosis measures the heaviness of the tails of a probability distribution compared to the tails of a normal distribution. It provides information about the presence of extreme values (outliers) and the sharpness of the distribution peak:

- $\textbf{Leptokurtic:}$ Positive excess kurtosis ($\gamma_2 > 0$) indicates a leptokurtic distribution, which has heavier tails and a sharper peak compared to a normal distribution.
- $\textbf{Mesokurtic:}$ A normal distribution has zero excess kurtosis ($\gamma_2 = 0$) and is referred to as mesokurtic. It means the tails are similar to those of a normal distribution.
- $\textbf{Platykurtic:}$ Negative excess kurtosis ($\gamma_2 < 0$) indicates a platykurtic distribution, which has lighter tails and a flatter peak compared to a normal distribution.

Understanding the moments, skewness, and kurtosis of a dataset helps in better interpreting the data's distribution and making informed decisions in various fields such as finance, economics, and data analysis.

## Correlation

Correlation is a statistical measure that quantifies the strength and direction of the linear relationship between two variables. It helps us understand how changes in one variable are associated with changes in another variable. Correlation is essential for determining the degree to which two variables move together or in opposite directions.

### Pearson Correlation Coefficient

The most common method of measuring correlation is the Pearson correlation coefficient ($r$). It ranges from -1 to 1, where:

- $r = 1$ indicates a perfect positive correlation (both variables increase together linearly).
- $r = -1$ indicates a perfect negative correlation (as one variable increases, the other decreases linearly).
- $r = 0$ indicates no linear correlation (the variables are not linearly related).

### Spearman and Kendall Correlation

In cases where the relationship between variables is not linear, Spearman and Kendall correlation coefficients are used. Spearman correlation calculates the correlation between the ranks of data points, while Kendall correlation measures the similarity of the ordering of data points.

### Interpreting Correlation

It's essential to remember that correlation does not imply causation. A high correlation between two variables does not necessarily mean one variable causes the other to change. Causality requires additional analysis and experiments.

## Regression

Regression is a statistical technique used to model the relationship between a dependent variable (response) and one or more independent variables (predictors). It enables us to make predictions and understand how the dependent variable changes as the independent variables vary.

### Linear Regression

Linear regression is the most common form of regression. It aims to fit a straight line (linear equation) to the data points that best describes the relationship between the dependent and independent variables. The equation of a simple linear regression model is of the form:

$$
y = \beta_0 + \beta_1 \cdot x + \varepsilon
$$

where:

- $y$ is the dependent variable,
- $x$ is the independent variable,
- $\beta_0$ is the intercept (y-value when $x$ is 0),
- $\beta_1$ is the slope (change in $y$ for a unit change in $x$),
- $\varepsilon$ represents the error term (residuals, the difference between the predicted and actual values).

### Multiple Regression

In cases with more than one independent variable, multiple regression is used. It extends the linear regression model to accommodate multiple predictors. The equation becomes:

$$
y = \beta_0 + \beta_1 \cdot x_1 + \beta_2 \cdot x_2 + \ldots + \beta_n \cdot x_n + \varepsilon
$$

### Interpreting Regression

Regression analysis helps us understand the relationship between variables, predict outcomes, and identify which independent variables are significant predictors of the dependent variable. It is widely used in various fields, including economics, finance, social sciences, and machine learning.

### Assumptions

It is crucial to check the assumptions of regression, such as linearity, independence of errors, constant variance of residuals (homoscedasticity), and normality of residuals, to ensure the validity and reliability of the regression model.

### Important Note

Correlation and regression are powerful tools, but they should be used carefully and complemented with other analyses to draw meaningful conclusions and make informed decisions based on the data.

## Rank Correlation

Rank correlation is a statistical measure used to assess the strength and direction of the association between two variables when the relationship is not linear. It is particularly useful when the data is ordinal, meaning that the variables are ranked or placed in categories with a natural order but no specific numeric value.

There are two commonly used methods for calculating rank correlation:

### Spearman Rank Correlation Coefficient (Spearman's $\rho$)

Spearman's rank correlation coefficient is based on the ranks of the data points rather than their actual values. It measures the extent to which the ranks of the data pairs move together or in opposite directions.

Suppose we have two variables, $X$ and $Y$, with corresponding ranks, $R_X$ and $R_Y$, and $n$ data points. The formula for calculating Spearman's rank correlation coefficient ($\rho$) is given by:

$$
\begin{equation*}
\rho = 1 - \frac{6\sum{d_i^2}}{n(n^2-1)}
\end{equation*}
$$

where $d_i$ is the difference between the ranks of the data pairs ($R_X - R_Y$) for each $i$-th data point.

The Spearman rank correlation coefficient ranges from $-1$ to $1$, where:

- $\rho = 1$ indicates a perfect positive rank correlation (the ranks of both variables are exactly the same).
- $\rho = -1$ indicates a perfect negative rank correlation (the ranks of one variable are the reverse of the ranks of the other variable).
- $\rho = 0$ indicates no rank correlation (the ranks are independent of each other).

### Kendall Rank Correlation Coefficient (Kendall's $\tau$)

Kendall's tau is another rank correlation measure that quantifies the similarity of the ordering of data points between two variables. It compares the number of concordant and discordant pairs of data.

Suppose we have two variables, $X$ and $Y$, with $n$ data points. The formula for calculating Kendall's tau ($\tau$) is given by:

$$
\begin{equation*}
\tau = \frac{\text{Number of concordant pairs} - \text{Number of discordant pairs}}{\frac{n(n-1)}{2}}
\end{equation*}
$$

The value of Kendall's tau ranges from $-1$ to $1$, where:

- $\tau = 1$ indicates a perfect positive rank correlation (all data pairs are concordant).
- $\tau = -1$ indicates a perfect negative rank correlation (all data pairs are discordant).
- $\tau = 0$ indicates no rank correlation (the number of concordant and discordant pairs are equal).

Rank correlation is particularly useful when dealing with data that cannot be measured on a continuous scale and may not follow a linear relationship. It provides a non-parametric measure of association, making it robust to outliers and resistant to certain types of data transformations. Rank correlation is widely used in fields such as sociology, psychology, and market research, where the data is often ranked or categorized.

