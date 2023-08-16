# $Continuous\,Probability\,Distributions$

---
A continuous probability distribution function, also known as a probability density function (PDF), describes the probability distribution of a continuous random variable $x$. Unlike discrete random variables, which can only take on specific isolated values, continuous random variables can take on any value within a certain range.

The properties of a continuous probability distribution function are as follows:

1. Non-Negativity: The probability density function is non-negative for all values of $x$:

$$
f(x) \geq 0 \quad \text{for all } x
$$

2. Total Area Under the Curve: The total area under the PDF curve over the entire range is equal to 1, representing the probability of the random variable falling within that range:

$$
\int_{-\infty}^{\infty} f(x) \, dx = 1
$$

3. Probability of a Range: The probability that the random variable $x$ falls within a specific range $a \leq x \leq b$ is given by the integral of the PDF over that range:

$$
P(a \leq x \leq b) = \int_{a}^{b} f(x) \, dx
$$

The cumulative distribution function (CDF) is another important concept related to the PDF. It gives the probability that the random variable $x$ is less than or equal to a given value $x_0$:

$$
F(x_0) = P(X \leq x_0) = \int_{-\infty}^{x_0} f(x) \, dx
$$

Examples of Continuous Probability Distribution Functions:

1. Normal Distribution (Gaussian Distribution).
2. Uniform Distribution.
3. Exponential Distribution.

These are just a few examples, and there are many other continuous probability distribution functions used to model various phenomena in different fields of study. Understanding these distributions and their properties is essential for statistical analysis and probability modelling.

**$\Rightarrow$ Visualizing the Probability Density Function of a Random Variable**

The probability density function of a random variable X is given by:
$\,$

<iframe scrolling="no" title="continuous probability question" src="https://www.geogebra.org/material/iframe/id/hq78h24r" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

## Example:

Suppose you have a continuous random variable $x$ representing the time (in hours) that a student spends studying for a statistics exam. The probability density function (PDF) of this variable is given by:

$$
f(x) = \frac{1}{3}e^{-\frac{x}{3}} \quad \text{for } x \geq 0
$$

a) Verify that the given function is a valid probability density function (PDF).

b) Find the probability that a student spends between 2 to 5 hours studying for the exam.

c) Calculate the cumulative distribution function (CDF) for $x$.

d) What is the probability that a student spends less than 4 hours studying for the exam?

e) If a student is chosen at random, what is the probability that they spend more than 6 hours studying for the exam?

+++ **Solution**

**a)** To verify that the given function is a valid probability density function, we need to check the following properties:

- Non-negativity: $f(x) \geq 0$ for all $x \geq 0$.
- Total area under the curve: $\int_{0}^{\infty} f(x) \, dx = 1$.

The function $f(x) = \frac{1}{3}e^{-\frac{x}{3}}$ is non-negative for all $x \geq 0$. Now, let's calculate the total area under the curve:

$$
\int_{0}^{\infty} \frac{1}{3}e^{-\frac{x}{3}} \, dx
$$

To evaluate this integral, we can use the fact that $\int e^{-at} \, dt = -\frac{1}{a}e^{-at} + C$.

So,

$$
\int_{0}^{\infty} \frac{1}{3}e^{-\frac{x}{3}} \, dx = \left[-\frac{1}{3}e^{-\frac{x}{3}} \right]_{0}^{\infty}
$$

Evaluating at the limits:

$$
\left[-\frac{1}{3}e^{-\frac{x}{3}} \right]_{0}^{\infty} = -\frac{1}{3}e^{-\frac{\infty}{3}} - \left(-\frac{1}{3}e^{-\frac{0}{3}}\right)
$$

Since $e^{-\infty}$ approaches zero, we have:

$$
\left[-\frac{1}{3}e^{-\frac{x}{3}} \right]_{0}^{\infty} = \frac{1}{3}
$$

Thus, the total area under the curve is 1, which confirms that the given function is a valid probability density function.

**b)** To find the probability that a student spends between 2 to 5 hours studying for the exam, we need to calculate:

$$
P(2 \leq x \leq 5) = \int_{2}^{5} \frac{1}{3}e^{-\frac{x}{3}} \, dx
$$

Using the same integration technique as before:

$$
P(2 \leq x \leq 5) = \left[-\frac{1}{3}e^{-\frac{x}{3}} \right]_{2}^{5} = -\frac{1}{3}e^{-\frac{5}{3}} + \frac{1}{3}e^{-\frac{2}{3}}
$$

Calculating the numerical value:

$$
P(2 \leq x \leq 5) \approx 0.184
$$

So, the probability that a student spends between 2 to 5 hours studying for the exam is approximately 0.184.

**c)** The cumulative distribution function (CDF) for $x$ is given by:

$$
F(x) = \int_{-\infty}^{x} f(t) \, dt
$$

For our PDF $f(x) = \frac{1}{3}e^{-\frac{x}{3}}$, the CDF is:

$$
F(x) = \int_{0}^{x} \frac{1}{3}e^{-\frac{t}{3}} \, dt
$$

Using the integration technique, we get:

$$
F(x) = \left[-\frac{1}{3}e^{-\frac{t}{3}} \right]_{0}^{x} = -\frac{1}{3}e^{-\frac{x}{3}} + \frac{1}{3}
$$

So, the cumulative distribution function for $x$ is:

$$
F(x) = 1 - e^{-\frac{x}{3}}
$$

**d)** To find the probability that a student spends less than 4 hours studying for the exam, we can use the CDF calculated in part-c

$$
P(x < 4) = F(4) = 1 - e^{-\frac{4}{3}} \approx 0.63
$$

Thus, the probability that a student spends less than 4 hours studying for the exam is approximately 0.63.

**e)** To calculate the probability that a student spends more than 6 hours studying for the exam, we can use the complement rule:

$$
P(x > 6) = 1 - P(x \leq 6) = 1 - F(6) = 1 - (1 - e^{-\frac{6}{3}}) = e^{-2} \approx 0.135
$$

So, the probability that a student spends more than 6 hours studying for the exam is approximately 0.135.

+++
$\,$
$\,$

## Expectation (E) of a Continuous Random Variable

In probability theory, the expectation of a continuous random variable is a fundamental concept that represents the average value or mean of the variable under its probability distribution. It is also commonly referred to as the expected value. The expectation is a measure of the central tendency of the random variable, providing valuable insights into its typical or most likely value.

For a continuous random variable $X$, the expectation $E(X)$ is calculated by taking the weighted average of all possible values that $X$ can take, where the weights are determined by the probability density function (PDF) of $X$. The concept of expectation allows us to summarize the behavior of the random variable in a single numerical value.
For a continuous random variable $X$ with probability density function $f(x)$, the expectation $E(X)$ is calculated as the integral of $X$ multiplied by its probability density function over the entire range of $X$:

$$
E(X) = Mean(\mu)=\int [X \cdot f(x)] dx
$$

Here, $E(X)$ represents the expectation or expected value of the continuous random variable $X$. The integral $\int$ is taken over the entire range of $X$, and the product of $X$ and $f(x)$ is integrated with respect to the variable $x$.

**Expectation of $X^2$ (E($X^2$)) for a Continuous Random Variable:**

For a continuous random variable $X$ with probability density function $f(x)$, the expectation of $X^2$ (E($X^2$)) is calculated as the integral of $X^2$ multiplied by its probability density function over the entire range of $X$:

$$
E(X^2) = \int [X^2 \cdot f(x)] dx
$$

**Variance (Var) for a Continuous Random Variable:**

The variance (Var) of a continuous random variable $X$ measures the spread or dispersion of $X$ around its expectation $E(X)$. It is calculated as follows:

$$
Var(X) = E(X^2) - [E(X)]^2
$$

**Expectation of a Function of a Random Variable ($E(f(X))$) for a Continuous Random Variable:**

For a function $f(X)$ of a continuous random variable $X$ with probability density function $f(x)$, the expectation of $f(X)$ ($E(f(X))$) is calculated as follows:

$$
E(f(X)) = \int [f(x) \cdot f(x)] dx
$$

$\,$
$\,$

## Moment Generating Function (MGF) for Continuous Distribution

The Moment Generating Function (MGF) for a continuous random variable is a mathematical function that uniquely characterizes the random variable and provides a way to find its moments. It is defined as the expected value of the exponential function raised to the power of the random variable multiplied by a constant $t$. For a continuous random variable $X$ with probability density function (PDF) $f(x)$, the MGF is given by:

$$
M_X(t) = E[e^{tX}] = \int_{-\infty}^{\infty} e^{tx} \cdot f(x) \, dx
$$

where the integration is taken over the entire range of the random variable $X$.

The MGF has several important properties:

1. The MGF is defined for all values of $t$ in an interval containing zero.
2. The $n$th moment of the random variable can be obtained by differentiating the MGF $n$ times with respect to $t$ and setting $t = 0$. Specifically, the $n$th moment is given by $E[X^n] = M_X^{(n)}(0)$, where $M_X^{(n)}(0)$ represents the $n$th derivative of $M_X(t)$ evaluated at $t = 0$.
3. If the MGF exists and is finite in a neighborhood of zero, then it uniquely determines the probability distribution of the random variable $X$.

The MGF is particularly useful in finding moments of a random variable, especially in cases where finding the moments directly from the PDF may be difficult or cumbersome. The MGF can be applied to various types of continuous distributions, including the normal distribution, exponential distribution, gamma distribution, and many others.

However, it's important to note that not all continuous random variables have a valid MGF for all values of $t$, especially when the distribution lacks certain moments or the MGF does not converge in certain regions.

| **Statistic** | **Formula** |
| :---: | :---: |
| Mean | $E(X) = \int [X \cdot f(x)] dx$ |
| Median | (For symmetric distributions, the median is the same as the mean) |
| Mode | (The mode is the value of $x$ that maximizes the probability density function $f(x)$) |
| Variance | $Var(X) = E(X^2) - [E(X)]^2$ |
| Standard Deviation | $SD(X) = \sqrt{Var(X)}$ |


**$\Rightarrow$ This allows you to investigate Probability Density Functions (PDFs)**

Enter a PDF in the f(x) input box and the range it operates on underneath.
(note this applet works only for single finite ranges).
$\,$
<iframe scrolling="no" title="Expectation" src="https://www.geogebra.org/material/iframe/id/ndngjmsz" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

## Linearity of Expectation

The linearity of expectation is a fundamental property that holds for both discrete and continuous random variables. It states that the expectation (or mean) of a linear combination of random variables is equal to the linear combination of their individual expectations.

For any constants $a$ and $b$ and any random variables $X$ and $Y$, the linearity of expectation can be expressed as follows:

1. For a single random variable $X$:

$$
E[aX + b] = aE[X] + b
$$

2. For multiple random variables $X$ and $Y$:

$$
E[aX + bY] = aE[X] + bE[Y]
$$

The linearity of expectation is a powerful property that simplifies the calculation of the expected value when dealing with combinations of random variables. It allows us to break down complex expressions into simpler components and compute their expectations separately.

**Question:**

A continuous random variable $X$ is described by the probability density function (PDF) given by:

$$
f(x) = \begin{cases} 
      \frac{2}{9}x & 0 \leq x \leq 3 \\
      0 & \text{otherwise} 
   \end{cases}
$$

Calculate the following:

a) The expectation ($E[X]$) of the random variable $X$.

b) The expectation ($E[X^2]$) of the random variable $X^2$.

c) The variance ($Var(X)$) of the random variable $X$.

d) The expectation ($E[f(X)]$) of the function $f(X) = 2X + 1$.

+++ **Solution:**

a) The expectation ($E[X]$) of a continuous random variable $X$ is calculated by integrating the product of the variable $X$ and its probability density function (PDF) over the entire range of possible values.

For the given probability density function $f(x)$, we have:

$$
E[X] = \int_{-\infty}^{\infty} x \cdot f(x) \, dx
$$

Since $f(x) = 0$ for $x < 0$ and $x > 3$, we can limit the integration to the range where $f(x)$ is nonzero, which is from 0 to 3.

$$
E[X] = \int_{0}^{3} x \cdot \left(\frac{2}{9}x\right) \, dx
$$

Now, we can perform the integration:

$$
E[X] = \frac{2}{9} \int_{0}^{3} x^2 \, dx
$$

$$
E[X] = \frac{2}{9} \left[\frac{x^3}{3}\right]_{0}^{3}
$$

$$
E[X] = \frac{2}{9} \left(\frac{3^3}{3} - \frac{0^3}{3}\right)
$$

$$
E[X] = \frac{2}{9} \cdot 9
$$

$$
E[X] = 2
$$

Therefore, the expectation ($E[X]$) of the random variable $X$ is 2.

b) To find the expectation ($E[X^2]$), we follow a similar approach:

$$
E[X^2] = \int_{-\infty}^{\infty} x^2 \cdot f(x) \, dx
$$

Since $f(x) = 0$ for $x < 0$ and $x > 3$, we integrate over the range from 0 to 3:

$$
E[X^2] = \int_{0}^{3} x^2 \cdot \left(\frac{2}{9}x\right) \, dx
$$

$$
E[X^2] = \frac{2}{9} \int_{0}^{3} x^3 \, dx
$$

$$
E[X^2] = \frac{2}{9} \left[\frac{x^4}{4}\right]_{0}^{3}
$$

$$
E[X^2] = \frac{2}{9} \left(\frac{3^4}{4} - \frac{0^4}{4}\right)
$$

$$
E[X^2] = \frac{2}{9} \cdot \frac{81}{4}
$$

$$
E[X^2] = \frac{9}{2}
$$

Therefore, the expectation ($E[X^2]$) of the random variable $X^2$ is $\frac{9}{2}$.

c) The variance ($Var(X)$) of a random variable $X$ is defined as:

$$
Var(X) = E[X^2] - (E[X])^2
$$

From parts (a) and (b), we have:

$$
Var(X) = \frac{9}{2} - 2^2
$$

$$
Var(X) = \frac{9}{2} - 4
$$

$$
Var(X) = \frac{1}{2}
$$

Therefore, the variance ($Var(X)$) of the random variable $X$ is $\frac{1}{2}$.

d) To find the expectation ($E[f(X)]$) of the function $f(X) = 2X + 1$, we apply the transformation to the random variable $X$ and calculate its expectation:

$$
E[f(X)] = E[2X + 1]
$$

Using linearity of expectation:

$$
E[f(X)] = 2E[X] + E[1]
$$

From part (a),

$$
E[f(X)] = 2\times2 + 1
$$

$$
E[f(X)] = 5
$$

+++
$\,$
$\,$

## Normal Distribution $X\sim N(\mu,\sigma ^{2})$

The normal distribution, also known as the Gaussian distribution, is one of the most widely used probability distributions in statistics. It is a continuous distribution characterized by a symmetric bell-shaped curve. The shape of the curve is determined by two parameters: the mean ($\mu$) and the standard deviation ($\sigma$).

The probability density function (PDF) of the normal distribution is given by:

$$
f(x) = \frac{1}{{\sigma \sqrt{2\pi}}} \exp\left(-\frac{(x-\mu)^2}{2\sigma^2}\right)
$$

where:

- $x$ is the random variable.
- $\mu$ is the mean or expected value, which represents the center of the distribution.
- $\sigma$ is the standard deviation, which measures the spread or dispersion of the data.
- $\pi$ is a mathematical constant (approximately 3.14159).

The normal distribution is characterized by the following properties:

1. It is symmetric around the mean $\mu$.
2. The curve reaches its maximum at $x = \mu$.
3. The total area under the curve is equal to 1, representing the probabilities of all possible outcomes.

Applications of the normal distribution include modeling of measurement errors, natural phenomena, financial data, and many other real-world processes. Its widespread use is due to its mathematical tractability and its ability to model a wide range of data with just two parameters.

<iframe scrolling="no" title="Normal Distribution&Standard Normal distributon" src="https://www.geogebra.org/material/iframe/id/sbxu2d4e" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

The **standard normal distribution**, denoted by $Z \sim \mathcal{N}(0, 1)$, is a special case of the normal distribution with a mean $\mu=0$ and a standard deviation $\sigma=1$. It has the probability density function:

$$
\phi(z) = \frac{1}{\sqrt{2\pi}} \cdot e^{-\frac{z^2}{2}}
$$

To convert a value $x$ from a normal distribution ($X$) to a standard normal distribution ($Z$), we use the transformation called standardization or normalization. The formula for this transformation is known as the z-score formula:

$$
Z = \frac{X - \mu}{\sigma}
$$

where:

- $X$ is the value from the original normal distribution,
- $\mu$ is the mean of the original normal distribution,
- $\sigma$ is the standard deviation of the original normal distribution, and
- $Z$ is the transformed value representing the z-score in the standard normal distribution.

The z-score, $Z$, represents the number of standard deviations the original value $X$ is from the mean $\mu$ of the original distribution. If $Z$ is positive, the $X$ value is above the mean; if it is negative, the $X$ value is below the mean.

The standard normal distribution is particularly useful because it simplifies various calculations and allows us to use standard normal distribution tables or statistical software to find probabilities and percentiles for specific z-scores. These tables and software provide the cumulative probabilities, allowing us to determine the probability of obtaining values within a certain range or greater than a specific value in a normal distribution without explicitly calculating integrals.

In summary, converting a normal distribution to a standard normal distribution involves standardizing data using the z-score formula. This transformation is valuable in statistical analysis, hypothesis testing, and making comparisons across different normal distributions, as it allows us to work with a common standardized scale.

**Question:**
The heights of adult male students in a university are normally distributed with a mean of 175 cm and a standard deviation of 7 cm.

a) What percentage of male students have heights between 165 cm and 185 cm?

b) If the university sets a height requirement of being in the top 10\% of male students, what is the minimum height a male student must have to meet this requirement?

+++ **Solution:**

a) To find the percentage of male students with heights between 165 cm and 185 cm, we will use the properties of the normal distribution. Let's first standardize the values using the z-score formula:

$$
z = \frac{x - \mu}{\sigma}
$$

where:

- $x$ is the height value,
- $\mu$ is the mean height (175 cm),
- $\sigma$ is the standard deviation (7 cm), and
- $z$ is the z-score.

For $x = 165$ cm:

$$
z_1 = \frac{165 - 175}{7} = -1.43
$$

For $x = 185$ cm:

$$
z_2 = \frac{185 - 175}{7} = 1.43
$$

Now, we need to find the area under the standard normal curve between $z_1$ and $z_2$. We can use a standard normal distribution table or a calculator to find these values. Since the normal distribution is symmetric, the area between $z_1$ and $z_2$ is the same as the area between $-z_2$ and $-z_1$. Therefore, we find the area for $z = 1.43$ and then subtract it from 1:

$$
P(-1.43 < z < 1.43) = 1 - 2 \times P(z > 1.43)
$$

Using a standard normal distribution table or calculator, we find $P(z > 1.43) \approx 0.0764$.

$$
P(-1.43 < z < 1.43) \approx 1 - 2 \times 0.0764 \approx 0.8472
$$

<iframe scrolling="no" title="Standard Normal Distribution calculatior" src="https://www.geogebra.org/material/iframe/id/muywqbff" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

So, approximately 84.72\% of male students have heights between 165 cm and 185 cm.

b) To find the minimum height a male student must have to be in the top 10\% of male students, we need to find the z-score corresponding to the 90th percentile. In other words, we need to find the z-score such that $P(z < z_{\text{score}}) = 0.90$.

Using a standard normal distribution table or calculator, we find the z-score corresponding to the 90th percentile is approximately 1.28.

Now, we can use the z-score formula to find the height corresponding to this z-score:

$$
z_{\text{score}} = \frac{x - 175}{7}
$$

$$
1.28 = \frac{x - 175}{7}
$$

Solving for $x$:

$$
x - 175 = 1.28 \times 7
$$

$$
x \approx 184
$$

So, the minimum height a male student must have to meet the university's requirement of being in the top 10\% of male students is approximately 184 cm.
+++
$\,$

**Question:**
The amount of time it takes a factory worker to assemble a particular product is normally distributed with a mean of 20 minutes and a standard deviation of 3 minutes.

a) What percentage of the workers take more than 25 minutes to assemble the product?
b) If the factory wants to identify the fastest 20\% of workers, what is the maximum time a worker can take to be in this category?

+++ **Solution:**

a) To find the percentage of workers who take more than 25 minutes to assemble the product, we use the properties of the normal distribution. Let's first standardize the value using the z-score formula:

$$
z = \frac{x - \mu}{\sigma}
$$

where:

- $x$ is the time taken to assemble the product (in minutes),
- $\mu$ is the mean time (20 minutes),
- $\sigma$ is the standard deviation (3 minutes), and
- $z$ is the z-score.

For $x = 25$ minutes:

$$
z = \frac{25 - 20}{3} = 1.67
$$

Now, we need to find the area under the standard normal curve to the right of this z-score (since we want values greater than 25 minutes). We can use a standard normal distribution table or a calculator to find this area.

$$
P(z > 1.67)
$$

Using a standard normal distribution table or calculator, we find $P(z > 1.67) \approx 0.0475$.

So, approximately 4.75\% of workers take more than 25 minutes to assemble the product.

b) To find the maximum time a worker can take to be in the fastest 20\% of workers, we need to find the z-score corresponding to the 80th percentile. In other words, we need to find the z-score such that $P(z < z_{\text{score}}) = 0.80$.

Using a standard normal distribution table or calculator, we find the z-score corresponding to the 80th percentile is approximately 0.84.

Now, we can use the z-score formula to find the time corresponding to this z-score:

$$
z_{\text{score}} = \frac{x - 20}{3}
$$

$$
0.84 = \frac{x - 20}{3}
$$

Solving for $x$:

$$
x - 20 = 0.84 \times 3
$$

$$
x \approx 22.52
$$

So, the maximum time a worker can take to be in the fastest 20\% of workers is approximately 22.52 minutes.
+++

## Gamma Distribution

The gamma distribution is a continuous probability distribution that is commonly used to model positive-valued random variables. It is a flexible distribution that can represent a wide range of shapes, making it useful in various statistical applications.

The probability density function (PDF) of the gamma distribution is given by:

$$
f(x) = \frac{1}{\Gamma(k) \cdot \theta^k} \cdot x^{k-1} \cdot e^{-\frac{x}{\theta}}
$$

where:

- $x \geq 0$ is the random variable.
- $k > 0$ is the shape parameter.
- $\theta > 0$ is the scale parameter.
- $\Gamma(k)$ is the gamma function, which is a generalization of the factorial for non-integer values.

<iframe scrolling="no" title="gamma distribution" src="https://www.geogebra.org/material/iframe/id/ecepwbnp" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

The gamma distribution includes several special cases, such as the exponential distribution (when $k = 1$), the chi-squared distribution (when $k$ is an integer), and the Erlang distribution (when $k$ is an integer and represents the number of events in an interval).

The mean and variance of the gamma distribution are $k \cdot \theta$ and $k \cdot \theta^2$, respectively.

The gamma distribution is often used to model the time between events in queuing systems, the lifetime of certain materials, and the waiting time for arrival processes, among other applications.

To fit the gamma distribution to data or estimate its parameters, various statistical methods such as maximum likelihood estimation (MLE) and method of moments can be used. The gamma distribution is widely supported in statistical software packages and provides a valuable tool for modeling positive-valued random variables in various fields of study.

## Exponential Distribution

The exponential distribution is a continuous probability distribution commonly used to model the time between events in a Poisson process. It is often employed to describe the waiting times between successive events when events occur at a constant rate independently of the time since the last event.

The probability density function (PDF) of the exponential distribution is given by:

$$
f(x) = \lambda e^{-\lambda x}
$$

where:

- $x \geq 0$ is the random variable representing the waiting time between events.
- $\lambda > 0$ is the rate parameter, which represents the average number of events occurring per unit of time.

The cumulative distribution function (CDF) of the exponential distribution is:

$$
F(x) = 1 - e^{-\lambda x}
$$

The mean (expected value) and variance of the exponential distribution are both $\frac{1}{\lambda}$.

<iframe scrolling="no" title="Exponential distribution" src="https://www.geogebra.org/material/iframe/id/as2uncv8" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

The exponential distribution has the memoryless property, meaning that the probability of an event occurring in the next time interval is independent of how much time has already passed. This property is expressed as:

$$
P(X > s + t | X > s) = P(X > t)
$$

where $X$ is a random variable representing the waiting time between events, and $s$ and $t$ are non-negative time values.

The exponential distribution is used in various fields, including queuing theory, reliability analysis, telecommunications, and survival analysis, among others. It provides a simple and versatile model for situations involving the time between events occurring at a constant rate.

**Exponentiated Exponential Distribution (not in syllabus):**

The exponentiated exponential distribution is a continuous probability distribution that extends the exponential distribution by introducing an additional parameter. It is also known as the generalized exponential distribution or the double exponential distribution. The exponentiated exponential distribution has two parameters, $a$ and $\lambda$, representing the shape and rate parameters, respectively.

The probability density function (PDF) of the exponentiated exponential distribution is given by:

$$
f(x) = \frac{a \lambda}{2} \exp(-a \lambda |x|)
$$

where $x$ can be any real value.

<iframe scrolling="no" title="exponential distribution" src="https://www.geogebra.org/material/iframe/id/jr6v4ryc" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

The exponentiated exponential distribution allows for more flexibility in modeling data compared to the standard exponential distribution. The value of the parameter $a$ determines the shape of the distribution. When $a = 1$, the exponentiated exponential distribution reduces to the standard exponential distribution.

