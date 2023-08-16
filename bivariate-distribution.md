# $Bivariate\,Distribution$

---

## Joint Distribution Function for Discrete Random Variables

For discrete random variables, the joint distribution is described by the joint probability density function (joint PDF). For two discrete random variables $X$ and $Y$, their joint PDF is denoted as $f(x, y)$ and it represents the probability density of both $X$ and $Y$ taking on specific values $x$ and $y$ simultaneously.

The joint PDF $f(x, y)$ satisfies the following properties:

1. Non-Negativity: $f(x, y) \geq 0$ for all $x$ and $y$.
2. Total Probability: The sum of the joint probabilities over all possible values of $X$ and $Y$ equals 1:
$\sum_{x}\sum_{y} f(x, y) = 1$.

### Example

Consider two discrete random variables, $X$ and $Y$, representing the outcomes of two fair six-sided dice rolls. The joint distribution function for this scenario can be represented as follows:

| $F_{X, Y}(x, y)$ | 1 | 2 | 3 | 4 | 5 | 6 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| 1 | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ |
| 2 | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ |
| 3 | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ |
| 4 | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ |
| 5 | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ |
| 6 | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ | $\frac{1}{36}$ |


### Interpretation

In the above example, each cell in the table represents the joint probability of the outcomes $X$ and $Y$. For instance, the value in the cell corresponding to $X = 3$ and $Y = 4$ is $\frac{1}{36}$, indicating that the probability of getting $X = 3$ and $Y = 4$ simultaneously from the two dice rolls is $\frac{1}{36}$.

### Properties and Uses

The joint distribution function has several properties, such as non-negativity, monotonicity, and right continuity. It is fundamental in computing probabilities of specific events involving multiple random variables, analyzing dependencies between variables, and constructing probability distributions for statistical modelling.

In summary, the joint distribution function for discrete random variables provides valuable insights into the probabilities of various combinations of outcomes for multiple random variables. It is a crucial tool in probability theory and statistics, facilitating rigorous probabilistic analyses and modelling in a wide range of applications.

**Question:** Consider two discrete random variables $X$ and $Y$ with the following joint distribution function:

$$
F_{XY}(x, y) = 
\begin{cases}
0.1 & \text{for } x = 1 \text{ and } y = 2 \\
0.2 & \text{for } x = 1 \text{ and } y = 3 \\
0.3 & \text{for } x = 2 \text{ and } y = 2 \\
0.4 & \text{for } x = 2 \text{ and } y = 3 \\
0 & \text{otherwise}
\end{cases}
$$

Find the probability mass function (PMF) of $X$ and $Y$ individually.

+++ **Solution:**

The probability mass function (PMF) of a discrete random variable gives the probability that the random variable takes on each possible value. To find the PMFs of $X$ and $Y$, we need to calculate the individual probabilities for each value of $X$ and $Y$ based on the joint distribution function.

### PMF of $X$

To find the PMF of $X$, we sum the probabilities of all the values of $Y$ for each possible value of $X$:

For $X = 1$:
$P(X = 1) = F_{XY}(1,2) + F_{XY}(1,3) = 0.1 + 0.2 = 0.3$

For $X = 2$:
$P(X = 2) = F_{XY}(2,2) + F_{XY}(2,3) = 0.3 + 0.4 = 0.7$

The PMF of $X$ is given by:

$$
P(X) = 
\begin{cases}
0.3 & \text{for } X = 1 \\
0.7 & \text{for } X = 2 \\
0 & \text{for other values of } X
\end{cases}
$$

### PMF of $Y$

To find the PMF of $Y$, we sum the probabilities of all the values of $X$ for each possible value of $Y$:

For $Y = 2$:
$P(Y = 2) = F_{XY}(1,2) + F_{XY}(2,2) = 0.1 + 0.3 = 0.4$

For $Y = 3$:
$P(Y = 3) = F_{XY}(1,3) + F_{XY}(2,3) = 0.2 + 0.4 = 0.6$

The PMF of $Y$ is given by:

$$
P(Y) = 
\begin{cases}
0.4 & \text{for } Y = 2 \\
0.6 & \text{for } Y = 3 \\
0 & \text{for other values of } Y
\end{cases}
$$

+++
$\,$
$\,$
**Question:** Consider two discrete random variables $X$ and $Y$ with the joint probability mass function given by:

$$
f_{XY}(x, y) = 
\begin{cases}
cxy & \text{for } x = 1, 2 \text{ and } y = 1, 2 \\
0 & \text{otherwise}
\end{cases}
$$

where $c$ is a constant. Find the value of $c$ and calculate the probability mass function (PMF) of $X$ and $Y$ individually.

+++ **Solution:**

To find the value of $c$, we need to ensure that the sum of probabilities over all possible values of $X$ and $Y$ equals 1, as it must be for a valid probability mass function.

First, let's find the value of $c$:

The sum of probabilities over all possible values of $X$ and $Y$ must be 1:

$$
\begin{aligned}
1 &= \sum_{x=1}^{2} \sum_{y=1}^{2} f_{XY}(x, y) \\
&= c(1 \cdot 1) + c(1 \cdot 2) + c(2 \cdot 1) + c(2 \cdot 2) \\
&= 6c
\end{aligned}
$$

Therefore, $c = \frac{1}{6}$.

Now, let's calculate the probability mass function (PMF) of $X$ and $Y$ individually.

### PMF of $X$

To find the PMF of $X$, we sum the probabilities of all the values of $Y$ for each possible value of $X$:

For $X = 1$:
$P(X = 1) = f_{XY}(1, 1) + f_{XY}(1, 2) = \frac{1}{6} \cdot 1 \cdot 1 + \frac{1}{6} \cdot 1 \cdot 2 = \frac{1}{3}$

For $X = 2$:
$P(X = 2) = f_{XY}(2, 1) + f_{XY}(2, 2) = \frac{1}{6} \cdot 2 \cdot 1 + \frac{1}{6} \cdot 2 \cdot 2 = \frac{1}{3}$

The PMF of $X$ is given by:

$$
P(X) = 
\begin{cases}
\frac{1}{3} & \text{for } X = 1 \\
\frac{1}{3} & \text{for } X = 2 \\
0 & \text{for other values of } X
\end{cases}
$$

### PMF of $Y$

To find the PMF of $Y$, we sum the probabilities of all the values of $X$ for each possible value of $Y$:

For $Y = 1$:
$P(Y = 1) = f_{XY}(1, 1) + f_{XY}(2, 1) = \frac{1}{6} \cdot 1 \cdot 1 + \frac{1}{6} \cdot 2 \cdot 1 = \frac{1}{6} + \frac{1}{3} = \frac{1}{2}$

For $Y = 2$:
$P(Y = 2) = f_{XY}(1, 2) + f_{XY}(2, 2) = \frac{1}{6} \cdot 1 \cdot 2 + \frac{1}{6} \cdot 2 \cdot 2 = \frac{1}{3} + \frac{1}{3} = \frac{2}{3}$

The PMF of $Y$ is given by:

$$
P(Y) = 
\begin{cases}
\frac{1}{2} & \text{for } Y = 1 \\
\frac{2}{3} & \text{for } Y = 2 \\
0 & \text{for other values of } Y
\end{cases}
$$

In summary, the constant $c$ is $\frac{1}{6}$, and the probability mass functions (PMFs) of $X$ and $Y$ for the given joint probability mass function are as follows:

$P(X) = 
\begin{cases}
\frac{1}{3} & \text{for } X = 1 \\
\frac{1}{3} & \text{for } X = 2 \\
0 & \text{for other values of } X
\end{cases}$

$P(Y) = 
\begin{cases}
\frac{1}{2} & \text{for } Y = 1 \\
\frac{2}{3} & \text{for } Y = 2 \\
0 & \text{for other values of } Y
\end{cases}$

+++
$\,$
$\,$
**$\Rightarrow$From the joint PDF, we can derive marginal probability density functions, denoted as $f_X(x)$ and $f_Y(y)$, which provide the probabilities of each random variable independently.**

$\rightarrow$The marginal probability density function $f_X(x)$ of $X$ is obtained by summing the joint probabilities over all possible values of $Y$:

$$
f_X(x) = \sum_{y} f(x, y)
$$

$\rightarrow$Similarly, the marginal probability density function $f_Y(y)$ of $Y$ is derived by summing the joint probabilities over all possible values of $X$:

$$
f_Y(y) = \sum_{x} f(x, y)
$$

$\,$
$\,$
$\,$

## Joint Probability Density Function for Continuous Random Variables

For continuous random variables $X$ and $Y$, the joint probability density function (joint PDF) is denoted as $f(x, y)$ and represents the probability density of both $X$ and $Y$ simultaneously taking on specific values $x$ and $y$.

The joint PDF $f(x, y)$ satisfies the following properties:

**1.** Non-Negativity: $f(x, y) \geq 0$ for all $x$ and $y$.
**2.** Total Probability: The integral of the joint PDF over the entire plane equals 1:

## $\iint_{\mathbb{R}^2} f(x, y) \, dx \, dy = 1$.

The properties for the joint PDF of continuous random variables are analogous to those of the joint probability mass function (PMF) for discrete random variables. However, since continuous random variables take on an uncountably infinite number of possible values within a range, we use integrals instead of sums to calculate probabilities over the entire range of $X$ and $Y$.

**$\Rightarrow$From the joint PDF, we can obtain the marginal probability density functions, denoted as $f_X(x)$ and $f_Y(y)$, which provide the probabilities of each random variable independently.**

$\rightarrow$The marginal probability density function $f_X(x)$ of $X$ is derived by integrating the joint PDF over all possible values of $Y$:

$$
f_X(x) = \int_{-\infty}^{\infty} f(x, y) \, dy
$$

<iframe scrolling="no" title="marginal distribution" src="https://www.geogebra.org/material/iframe/id/nkcgh3ca" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

$\rightarrow$Similarly, the marginal probability density function $f_Y(y)$ of $Y$ is obtained by integrating the joint PDF over all possible values of $X$:

$$
f_Y(y) = \int_{-\infty}^{\infty} f(x, y) \, dx
$$

The concept of the joint PDF for continuous random variables is essential in probability theory and statistics, as it allows us to model and analyze the relationships between multiple continuous variables in various real-world applications.

**Question:** The joint probability density function (joint PDF) of two continuous random variables $X$ and $Y$ is given by:

$$
f(x, y) = 
\begin{cases}
kxy, & \text{for } 0 \leq x \leq 3 \text{ and } 1 \leq y \leq 4 \\
0, & \text{otherwise}
\end{cases}
$$

a) Find the value of $k$ such that $f(x, y)$ satisfies the property of total probability.

b) Calculate the probability $P(1 \leq x \leq 2, 2 \leq y \leq 3)$.

+++ **Solution:**

a) To find the value of $k$, we need to ensure that the joint PDF $f(x, y)$ satisfies the property of total probability, i.e., the integral over the entire plane equals 1:

$$
\iint_{\text{all space}} f(x, y) \, dx \, dy = 1
$$

Since the joint PDF is zero outside the range $0 \leq x \leq 3$ and $1 \leq y \leq 4$, the integral becomes:

$$
\int_{0}^{3} \int_{1}^{4} kxy \, dy \, dx = 1
$$

Evaluate the inner integral first:

$$
\int_{1}^{4} kxy \, dy = kx \int_{1}^{4} y \, dy = kx \left[\frac{1}{2}y^2\right]_{1}^{4} = kx \left(\frac{16}{2} - \frac{1}{2}\right) = 7kx
$$

Now, integrate with respect to $x$:

$$
\int_{0}^{3} 7kx \, dx = 7k \int_{0}^{3} x \, dx = 7k \left[\frac{1}{2}x^2\right]_{0}^{3} = 7k \cdot \frac{9}{2} = \frac{63}{2}k
$$

Setting this equal to 1:

$$
\frac{63}{2}k = 1
$$

$$
k = \frac{2}{63}
$$

Now, we have the value of $k$, which is $k = \frac{2}{63}$.

b) To calculate the probability $P(1 \leq x \leq 2, 2 \leq y \leq 3)$, we need to find the double integral of the joint PDF over the given region:

$$
P(1 \leq x \leq 2, 2 \leq y \leq 3) = \iint_{1 \leq x \leq 2, 2 \leq y \leq 3} \frac{2}{63} \cdot xy \, dy \, dx
$$

Evaluate the inner integral first:

$$
\int_{2}^{3} \frac{2}{63} \cdot xy \, dy = \frac{2}{63}x \int_{2}^{3} y \, dy = \frac{2}{63}x \left[\frac{1}{2}y^2\right]_{2}^{3} = \frac{2}{63}x \left(\frac{9}{2} - 2\right) = \frac{2}{63}x \cdot \frac{5}{2} = \frac{5}{63}x
$$

Now, integrate with respect to $x$:

$$
P(1 \leq x \leq 2, 2 \leq y \leq 3) = \int_{1}^{2} \frac{5}{63}x \, dx
$$

$$
P(1 \leq x \leq 2, 2 \leq y \leq 3) = \frac{5}{63} \int_{1}^{2} x \, dx
$$

$$
P(1 \leq x \leq 2, 2 \leq y \leq 3) = \frac{5}{63} \left[\frac{1}{2}x^2\right]_{1}^{2}
$$

$$
P(1 \leq x \leq 2, 2 \leq y \leq 3) = \frac{5}{63} \left(\frac{4}{2} - \frac{1}{2}\right)
$$

$$
P(1 \leq x \leq 2, 2 \leq y \leq 3) = \frac{5}{63} \cdot \frac{3}{2}
$$

$$
P(1 \leq x \leq 2, 2 \leq y \leq 3) = \frac{5}{126}
$$

Therefore, the probability $P(1 \leq x \leq 2, 2 \leq y \leq 3)$ is $\frac{5}{126}$ or approximately 0.0397.
+++
$\,$
**Question:** Suppose the joint probability density function of two random variables, $X$ and $Y$, is given by:

$$
f(x, y) = \begin{cases} 
      k(2x + y) & \text{for } 0 \leq x \leq 1, 0 \leq y \leq 2 \\
      0 & \text{otherwise}
   \end{cases}
$$

a) Find the value of constant $k$ that makes $f(x, y)$ a valid joint probability density function.

b) Calculate the marginal probability density functions, $f_X(x)$ and $f_Y(y)$, for random variables $X$ and $Y$ respectively.

c) Determine the probability that both $X$ and $Y$ are greater than 0.5, i.e., find $P(X > 0.5 \text{ and } Y > 0.5)$.

+++ **Solution:**

a) To find the value of constant $k$, we need to ensure that the joint probability density function $f(x, y)$ satisfies the properties of a valid joint density function. The total probability over the entire range of $X$ and $Y$ must equal 1. Hence, we evaluate the double integral of $f(x, y)$ over the given region and set it equal to 1:

$$
\int_{0}^{1} \int_{0}^{2} k(2x + y) \, dy \, dx = 1
$$

Evaluating the integral:

$$
\int_{0}^{1} \left[ kxy + \frac{1}{2}ky^2 \right]_{0}^{2} \, dx = 1
$$

$$
\int_{0}^{1} (2kx + 2k) \, dx = 1
$$

$$
\left[ kx^2 + 2kx \right]_{0}^{1} = 1
$$

$$
k + 2k = 1
$$

$$
3k = 1
$$

$$
k = \frac{1}{3}
$$

b) To find the marginal probability density functions $f_X(x)$ and $f_Y(y)$, we integrate $f(x, y)$ over the entire range of the other variable:

For $f_X(x)$:

$$
f_X(x) = \int_{-\infty}^{\infty} f(x, y) \, dy
$$

Since $f(x, y)$ is non-zero only when $0 \leq y \leq 2$, the integral is taken over this range:

$$
f_X(x) = \int_{0}^{2} \frac{1}{3}(2x + y) \, dy
$$

$$
f_X(x) = \left[ \frac{1}{3}(2xy + \frac{1}{2}y^2) \right]_{0}^{2}
$$

$$
f_X(x) = \frac{1}{3}(4x + 2)
$$

For $f_Y(y)$:

$$
f_Y(y) = \int_{-\infty}^{\infty} f(x, y) \, dx
$$

Since $f(x, y)$ is non-zero only when $0 \leq x \leq 1$, the integral is taken over this range:

$$
f_Y(y) = \int_{0}^{1} \frac{1}{3}(2x + y) \, dx
$$

$$
f_Y(y) = \left[ \frac{1}{3}(x^2 + xy) \right]_{0}^{1}
$$

$$
f_Y(y) = \frac{1}{3}(1 + y)
$$

c) To find the probability that both $X$ and $Y$ are greater than 0.5, we need to calculate the joint probability:

$$
P(X > 0.5 \text{ and } Y > 0.5) = \int_{0.5}^{1} \int_{0.5}^{2} \frac{1}{3}(2x + y) \, dy \, dx
$$

$$
P(X > 0.5 \text{ and } Y > 0.5) = \frac{1}{3} \int_{0.5}^{1} \left[ 2xy + \frac{1}{2}y^2 \right]_{0.5}^{2} \, dx
$$

$$
P(X > 0.5 \text{ and } Y > 0.5) = \frac{1}{3} \int_{0.5}^{1} (2x + 1) \, dx
$$

$$
P(X > 0.5 \text{ and } Y > 0.5) = \frac{1}{3} \left[ x^2 + x \right]_{0.5}^{1}
$$

$$
P(X > 0.5 \text{ and } Y > 0.5) = \frac{1}{3} \left( 1 + 1 - \left( \frac{1}{4} + \frac{1}{2} \right) \right)
$$

$$
P(X > 0.5 \text{ and } Y > 0.5) = \frac{5}{12}
$$

Therefore, the probability that both $X$ and $Y$ are greater than 0.5 is $\frac{5}{12}$.+++

$\,$
$\,$

## Conditional Density Function for Joint Distribution

The conditional density function (also known as the conditional probability density function or conditional PDF) is a fundamental concept used to describe the distribution of one random variable given the value of another random variable in a joint distribution. It allows us to model the relationship between two random variables and understand how one variable influences the other under specific conditions.

Let's consider two continuous random variables, $X$ and $Y$, with a joint probability density function $f(x, y)$. The conditional density function of $X$ given that $Y = y$, denoted as $f_{X|Y}(x|y)$, represents the density of $X$ when we have information about the value of $Y$ being equal to $y$.

The conditional density function is defined as:

$$
f_{X|Y}(x|y) = \frac{f(x, y)}{f_Y(y)}
$$

where:

- $f_{X|Y}(x|y)$ is the conditional density function of $X$ given $Y = y$.
- $f(x, y)$ is the joint probability density function of $X$ and $Y$.
- $f_Y(y)$ is the marginal probability density function of $Y$.

The conditional density function is helpful in various applications, such as predictive modeling, Bayesian statistics, and inference. It allows us to compute the probability of one random variable taking on a specific value given the knowledge of the value of another random variable. In the context of continuous distributions, the conditional density function can be used to find conditional probabilities within specific intervals or to compute conditional expectations and variances.

For discrete random variables, the concept of conditional probability mass function is used, and the definition is slightly different. In both cases, the conditional density function plays a crucial role in understanding the relationship between two random variables in a joint distribution.
$\,$
$\,$
**Question:**

Consider two continuous random variables $X$ and $Y$ with a joint probability density function given by:

$$
f(x, y) = 
\begin{cases}
6xy, & \text{for } 0 \leq x \leq 1 \text{ and } 0 \leq y \leq 2 \\
0, & \text{otherwise}
\end{cases}
$$

a) Determine the conditional density function $f_{X|Y}(x|y)$ of $X$ given that $Y = y$.

b) Find the conditional probability $P(X \leq 0.5 | Y = 1)$.

+++ **Solution:**

a) The conditional density function $f_{X|Y}(x|y)$ of $X$ given that $Y = y$ is given by:

$$
f_{X|Y}(x|y) = \frac{f(x, y)}{f_Y(y)}
$$

where $f(x, y)$ is the joint probability density function of $X$ and $Y$, and $f_Y(y)$ is the marginal probability density function of $Y$.

The marginal probability density function $f_Y(y)$ can be obtained by integrating the joint density function $f(x, y)$ with respect to $x$ over the entire range of $x$:

$$
f_Y(y) = \int_{0}^{1} 6xy \, dx
$$

$$
f_Y(y) = 6y \int_{0}^{1} x \, dx
$$

$$
f_Y(y) = 6y \left[\frac{1}{2}x^2\right]_{0}^{1}
$$

$$
f_Y(y) = 6y \cdot \frac{1}{2} = 3y
$$

Now, we can calculate the conditional density function $f_{X|Y}(x|y)$ by substituting the values of $f(x, y)$ and $f_Y(y)$ into the formula:

$$
f_{X|Y}(x|y) = \frac{6xy}{3y}
$$

$$
f_{X|Y}(x|y) = 2x
$$

Therefore, the conditional density function of $X$ given that $Y = y$ is $f_{X|Y}(x|y) = 2x$.

b) To find the conditional probability $P(X \leq 0.5 | Y = 1)$, we need to integrate the conditional density function $f_{X|Y}(x|y = 1)$ over the interval $[0, 0.5]$:

$$
P(X \leq 0.5 | Y = 1) = \int_{0}^{0.5} f_{X|Y}(x|y = 1) \, dx
$$

$$
P(X \leq 0.5 | Y = 1) = \int_{0}^{0.5} 2x \, dx
$$

$$
P(X \leq 0.5 | Y = 1) = \left[x^2\right]_{0}^{0.5}
$$

$$
P(X \leq 0.5 | Y = 1) = 0.5^2 - 0^2 = 0.25
$$

Therefore, the conditional probability $P(X \leq 0.5 | Y = 1)$ is 0.25.
+++

## Bivariate Normal Distribution

The bivariate normal distribution is a probability distribution for two continuous random variables that are jointly normally distributed. It is a special case of the multivariate normal distribution, which describes the joint distribution of multiple correlated random variables. In the bivariate normal distribution, the two variables are assumed to have a bivariate normal relationship, meaning their joint distribution is characterized by a bell-shaped, elliptical contour.

The bivariate normal distribution is fully defined by the means ($\mu_X$ and $\mu_Y$), standard deviations ($\sigma_X$ and $\sigma_Y$), and the correlation coefficient ($\rho$) between the two variables. The correlation coefficient determines the degree of linear relationship between $X$ and $Y$, ranging from -1 (perfect negative correlation) to 1 (perfect positive correlation). When $\rho = 0$, $X$ and $Y$ are uncorrelated.

The probability density function (PDF) of the bivariate normal distribution is given by:

$$
f(x, y) = \frac{1}{{2\pi \sigma_X \sigma_Y \sqrt{1-\rho^2}}} \exp\left( -\frac{1}{2(1-\rho^2)} \left[ \frac{(x-\mu_X)^2}{\sigma_X^2} - 2\rho\frac{(x-\mu_X)(y-\mu_Y)}{\sigma_X \sigma_Y} + \frac{(y-\mu_Y)^2}{\sigma_Y^2} \right] \right)
$$

where:

- $x$ and $y$ are the values of the two variables.
- $\mu_X$ and $\mu_Y$ are the means of $X$ and $Y$, respectively.
- $\sigma_X$ and $\sigma_Y$ are the standard deviations of $X$ and $Y$, respectively.
- $\rho$ is the correlation coefficient between $X$ and $Y$.

<iframe scrolling="yes" title=" Bivariate Normal Distribution" src="https://www.geogebra.org/material/iframe/id/uhwwhfua" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

The bivariate normal distribution is widely used in various fields, including statistics, econometrics, finance, and engineering, when dealing with two continuous variables that exhibit a linear relationship. It allows for modeling the joint distribution of two variables and understanding their correlation and dependence. The bivariate normal distribution is also essential in statistical modeling, hypothesis testing, and constructing confidence intervals for the parameters involved.

