## Curve Fitting by the Method of Least Squares

Curve fitting is a process of finding a mathematical model that best approximates a set of data points. The method of least squares is a widely used technique for curve fitting, aiming to minimize the sum of the squared differences between the observed data points and the values predicted by the model.

## Linear Curve Fitting

In linear curve fitting, we seek to find the best-fitting straight line that describes the relationship between the dependent variable $y$ and the independent variable $x$. The linear equation has the form:

$$
y = mx + b
$$

where:

- $m$ is the slope of the line, representing the rate of change of $y$ with respect to $x$.
- $b$ is the y-intercept, the value of $y$ when $x$ is 0.

**Adjust the slider for the best-fitting straight line**

<iframe scrolling="no" title="linear curve fitting" src="https://www.geogebra.org/material/iframe/id/yqtenfkr" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

Given a set of $n$ data points $(x_i, y_i)$, the objective of linear curve fitting is to find the values of $m$ and $b$ that minimize the sum of the squared residuals (differences between the actual $y_i$ and the predicted values $mx_i + b$):

$$
\begin{equation*}
\text{minimize} \sum_{i=1}^{n} \left(y_i - (mx_i + b)\right)^2
\end{equation*}
$$

+++ **Example:-**

Suppose we have the following set of data points representing the relationship between $x$ and $y$:

| $x$ | $y$ |
| :---: | :---: |
| 1 | 3 |
| 2 | 5 |
| 3 | 7 |
| 4 | 10 |
| 5 | 12 |


We want to find a linear equation of the form $y = mx + b$ that best fits this data.

**Solution:**

### Step 1: Set up the equations

The linear equation to fit the data is: $y = mx + b$. We want to find the values of $m$ and $b$ that minimize the sum of squared differences between the observed $y$-values and the predicted $y$-values from the equation.

For each data point $(x_i, y_i)$, we have the following equation:

$$
y_i = mx_i + b
$$

### Step 2: Formulate the system of equations

For our given data points, we have five equations:
$$
\begin{align*}
1. &\quad 3 = m \times 1 + b \\
2. &\quad 5 = m \times 2 + b \\
3. &\quad 7 = m \times 3 + b \\
4. &\quad 10 = m \times 4 + b \\
5. &\quad 12 = m \times 5 + b \\
\end{align*}
$$

### Step 3: Use the Method of Least Squares

The method of least squares involves finding the values of $m$ and $b$ that minimize the sum of the squares of the vertical distances (residuals) between the observed data points and the corresponding points on the fitted line.

To minimize the sum of squared residuals, we take the partial derivatives of the sum of squared residuals with respect to $m$ and $b$ and set them equal to zero. Solving these equations will give us the values of $m$ and $b$ that minimize the sum of squared residuals.

Let's define the sum of squared residuals (SSR) as:

$$
SSR = \sum_{i=1}^{5} (y_i - (mx_i + b))^2
$$

Taking partial derivatives and setting them equal to zero:

$$
\frac{\partial SSR}{\partial m} = 0
$$

$$
\frac{\partial SSR}{\partial b} = 0
$$

### Step 4: Solve for $m$ and $b$

By solving the above equations, we can obtain the values of $m$ and $b$ that minimize the sum of squared residuals.

After solving the system of equations, we get:

$$
m \approx 2.3
$$

$$
b \approx 0.6
$$

So, the best-fitting linear equation is: $y \approx 2.3x + 0.6$.

### Step 5: Plot the linear curve on a graph

To visualize the linear curve fit, we can plot it on a graph along with the original data points.

In conclusion, by using the method of least squares, we found the equation $y \approx 2.3x + 0.6$ that best fits the given data points.
+++
$\,$
$\,$
$\,$

## Solving Linear Curve Fitting by Simplified Approach

Let's consider a set of data points representing the relationship between an independent variable $x$ and a dependent variable $y$.

The general equation for a linear function is:

$$
y = mx + b
$$

where $m$ is the slope and $b$ is the y-intercept of the line.

**Step 1:** Calculate the necessary sums
Calculate the following sums from the given data:

- $\sum x$: The sum of all $x$-values in the dataset.
- $\sum y$: The sum of all $y$-values in the dataset.
- $\sum xy$: The sum of the products of each $x$-value and its corresponding $y$-value.
- $\sum x^2$: The sum of the squares of all $x$-values in the dataset.

**Step 2:** Calculate the slope ($m$) and y-intercept ($b$)
Using the following formulas, we can calculate the slope ($m$) and y-intercept ($b$) for the best-fitting line:

$$
m = \frac{n \sum xy - \sum x \sum y}{n \sum x^2 - (\sum x)^2}
$$

$$
b = \frac{\sum y - m \sum x}{n}
$$

where $n$ is the number of data points.

**Step 3:** Interpretation and plotting
The calculated values of $m$ and $b$ represent the slope and y-intercept of the best-fitting line that approximates the data. The best-fitting linear equation is then $y = mx + b$.

To visualize the linear curve fit, we can plot the line $y = mx + b$ on a graph along with the original data points.
+++ **EXAMPLE:-**
Suppose we have the following set of data points representing the relationship between $x$ and $y$:

| $x$ | $y$ |
| :---: | :---: |
| 1 | 3 |
| 2 | 5 |
| 3 | 7 |
| 4 | 10 |
| 5 | 12 |


We want to find a linear equation of the form $y = mx + b$ that best fits this data.

**Solution:-**
**Step 1:** Calculate the necessary sums
Calculate the following sums from the given data:

$$
\sum x, \quad \sum y, \quad \sum xy, \quad \sum x^2, \quad \text{and} \quad \sum y^2
$$

For the given data:

$$
\sum x = 1 + 2 + 3 + 4 + 5 = 15
$$

$$
\sum y = 3 + 5 + 7 + 10 + 12 = 37
$$

$$
\sum xy = (1 \times 3) + (2 \times 5) + (3 \times 7) + (4 \times 10) + (5 \times 12) = 134
$$

$$
\sum x^2 = 1 + 4 + 9 + 16 + 25 = 55
$$

$$
\sum y^2 = 9 + 25 + 49 + 100 + 144 = 327
$$

**Step 2:** Calculate the slope (m) and y-intercept (b)
The formula for the slope (m) is:

$$
m = \frac{n \sum xy - \sum x \sum y}{n \sum x^2 - (\sum x)^2}
$$

The formula for the y-intercept (b) is:

$$
b = \frac{\sum y - m \sum x}{n}
$$

where $n$ is the number of data points, which in this case is 5.

Using the values from Step 1, we get:

$$
m = \frac{5 \times 134 - 15 \times 37}{5 \times 55 - 15^2} \approx 2.3
$$

$$
b = \frac{37 - 2.3 \times 15}{5} \approx 0.6
$$

So, the best-fitting linear equation is: $y \approx 2.3x + 0.6$.

**Step 3:** Plot the linear curve on a graph
To visualize the linear curve fit, we can plot it on a graph along with the original data points.

In conclusion, by using the method of least squares, we found the equation $y \approx 2.3x + 0.6$ that best fits the given data points.
+++
$\,$
$\,$
$\,$
$\,$

## Polynomial Curve Fitting

Polynomial curve fitting involves fitting a polynomial equation of degree $n$ to the data points. The general form of a polynomial of degree $n$ is:

$$
y = a_nx^n + a_{n-1}x^{n-1} + \ldots + a_1x + a_0
$$

where $a_n, a_{n-1}, \ldots, a_0$ are the coefficients to be determined.

For polynomial curve fitting, the goal is to find the values of the coefficients $a_n, a_{n-1}, \ldots, a_0$ that minimize the sum of the squared residuals:

$$
\begin{equation*}
\text{minimize} \sum_{i=1}^{n} \left(y_i - \left(a_nx_i^n + a_{n-1}x_i^{n-1} + \ldots + a_1x_i + a_0\right)\right)^2
\end{equation*}
$$

<iframe scrolling="no" title="Polynomial curve fitting" src="https://www.geogebra.org/material/iframe/id/afhq3qzn" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>
This applet can be used to enter data, see the scatter plot and view two polynomial fittings in the data (for comparison), If only one fit is desired enter 0 for Degree of Fit2 (or Fit1). If a data value is wrongly entered, select the correct check box and use use appropriate correct button to delete the (last) wrongly entered value. Selecting  show fits check box displays equations as well as graphs. Selecting Instructions check box displays instructions.

$\,$
$\,$
$\,$
$\,$

## Nonlinear Curve Fitting

In cases where the relationship between the variables is nonlinear, a general nonlinear equation is used for curve fitting. The nonlinear equation may not have a simple analytical form, and its parameters need to be estimated from the data.

For nonlinear curve fitting, we have a model with parameters $\theta$ (e.g., $\theta_1, \theta_2, \ldots$). The goal is to find the values of $\theta$ that minimize the sum of the squared residuals:

$$
\begin{equation*}
\text{minimize} \sum_{i=1}^{n} \left(y_i - f(x_i, \theta)\right)^2
\end{equation*}
$$
where $f(x_i, \theta)$ is the function that relates $x_i$ and $y_i$ with the parameters $\theta$.

$\,$
$\,$
$\,$
$\,$

## Introduction to Hypothesis Testing

Hypothesis testing is a fundamental concept in statistics that allows us to make decisions about a population based on sample data. It helps us determine if there is enough evidence to support or reject a claim (hypothesis) about a population parameter.

### Key Components

1. $\textbf{Null Hypothesis (\(H_0\)):}$ This is the initial assumption that there is no significant difference or effect. It represents the status quo and is usually denoted by $H_0$.
2. $\textbf{Alternative Hypothesis (\(H_a\)):}$ This is the claim or statement we want to investigate and determine if there is enough evidence to support. It opposes the null hypothesis and is denoted by $H_a$.

### Types of Hypotheses

- $\textbf{One-Tailed (or One-Sided) Hypothesis:}$ This type of hypothesis test focuses on either a positive or negative effect. It is denoted as $H_a: \mu > \mu_0$ (right-tailed) or $H_a: \mu < \mu_0$ (left-tailed), where $\mu$ is the population mean and $\mu_0$ is the hypothesized value.
- $\textbf{Two-Tailed Hypothesis:}$ This type of hypothesis test is more general and looks for any significant difference, regardless of the direction. It is denoted as $H_a: \mu \neq \mu_0$.

### Steps for Hypothesis Testing

1. $\textbf{Formulate Hypotheses:}$ Define the null and alternative hypotheses based on the research question.
2. $\textbf{Select Significance Level (\(\alpha\)):}$ The significance level is the probability of rejecting the null hypothesis when it is actually true. Common choices include 0.05 (5\%) or 0.01 (1\%).
3. $\textbf{Choose a Test Statistic:}$ The choice of test statistic depends on the type of data and the specific hypothesis test.
4. $\textbf{Calculate the Test Statistic:}$ Using the sample data, compute the value of the test statistic.
5. $\textbf{Determine the Critical Region:}$ This is the region of extreme values of the test statistic that leads to the rejection of the null hypothesis.
6. $\textbf{Compare Test Statistic with Critical Value:}$ If the test statistic falls within the critical region, reject the null hypothesis. Otherwise, fail to reject the null hypothesis.

### Common Test Statistics

- $\textbf{Z-Test:}$ Used when the population standard deviation ($\sigma$) is known, and the sample size is sufficiently large.

Formula: $Z = \frac{\bar{X} - \mu}{\sigma/\sqrt{n}}$
- $\textbf{T-Test:}$ Used when the population standard deviation ($\sigma$) is unknown or the sample size is small ($n < 30$).

Formula (for one-sample t-test): $t = \frac{\bar{X} - \mu}{s/\sqrt{n}}$, where $s$ is the sample standard deviation.
- $\textbf{Chi-Square Test (\(\chi^2\)):}$ Used for categorical data to test independence or goodness of fit.

Formula: $\chi^2 = \sum \frac{(O - E)^2}{E}$, where $O$ is the observed frequency and $E$ is the expected frequency.
- $\textbf{F-Test:}$ Used to compare the variance of two or more samples.

Formula (for two-sample F-test): $F = \frac{s_1^2}{s_2^2}$, where $s_1^2$ and $s_2^2$ are the sample variances.

Remember, hypothesis testing helps us draw conclusions based on evidence from sample data. Always interpret the results in the context of the problem and use statistical significance as a guide for decision-making.

**Question:** A company claims that the average response time of their customer support team is 10 minutes. To test this claim, a random sample of 36 customer support interactions was taken, and the average response time was found to be 12 minutes, with a sample standard deviation of 3 minutes. Conduct a hypothesis test using a two-tailed Z-test at a 5\% significance level to determine if there is enough evidence to reject the company's claim.

+++ **Solution:-**

**Step 1:** Formulate Hypotheses

**Null Hypothesis ($H_0$):** The average response time of the customer support team is equal to 10 minutes.

$$
H_0: \mu = 10
$$

**Alternative Hypothesis ($H_a$):** The average response time of the customer support team is not equal to 10 minutes.

$$
H_a: \mu \neq 10
$$

**Step 2:** Select Significance Level

In this case, the significance level ($\alpha$) is given as 0.05 (5\%).

**Step 3:** Choose a Test Statistic

Since the population standard deviation is unknown, we will use the Z-test for the mean.

**Step 4:** Calculate the Test Statistic

The formula for the Z-test is:

$$
Z = \frac{\bar{X} - \mu}{\frac{\sigma}{\sqrt{n}}}
$$

where:
$\bar{X}$ = Sample mean (12 minutes)<br>
$\mu$ = Population mean under the null hypothesis (10 minutes)<br>
$\sigma$ = Population standard deviation (unknown)<br>
$n$ = Sample size (36)

**Step 5:** Determine the Critical Region

Since this is a two-tailed test, we need to find the critical Z-values for a 5\% significance level.

For a two-tailed test at 5\% significance level, we divide the significance level by 2 to get 2.5\% on each tail. Using a Z-table or calculator, we find the critical Z-values to be approximately -1.96 and +1.96.

**Step 6:** Compare Test Statistic with Critical Value

Calculate the test statistic:

$$
Z = \frac{12 - 10}{\frac{3}{\sqrt{36}}} = \frac{2}{\frac{3}{6}} = 4
$$

<iframe scrolling="no" title="two tail hypothesis Z-test" src="https://www.geogebra.org/material/iframe/id/f8tytbyf" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

Since the calculated Z-value (4) is greater than the critical Z-values (-1.96 and 1.96), we reject the null hypothesis.

**Step 7:** Conclusion

There is enough evidence to reject the company's claim that the average response time of their customer support team is 10 minutes. The data suggests that the average response time is significantly different from 10 minutes.
+++

