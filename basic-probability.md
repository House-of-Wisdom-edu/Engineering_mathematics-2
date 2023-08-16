# $Basic\,Probability$

----
Probability is a way to measure the chances of something happening. It helps us understand how likely or unlikely an event is. Probability ranges from 0 (impossible) to 1 (certain). It is used in many areas, like predicting the weather or winning a game. We can calculate probabilities by defining all possible outcomes and assigning numbers to represent their likelihood. It's a useful tool for making decisions when we're unsure about the outcome.

# Sets

You may omit this section if you are familiar with these concepts.

A set is a collection of **distinct** objects.

We often specify a set by listing its members, or elements, in parentheses like this {}. For example A = {2, 4, 6, 8} means that A is the set consisting of numbers 2,4,6,8. We could also write A ={even numbers less than 9}.

### Set Operations

- **Union:** The union of $A$ and $B$ is the set of elements which belong to $A$ or to $B$ (or both) and can be written as $A ∪ B$.
- **Intersection:** The intersection of $A$ and $B$ is the set of elements which belong to both $A$ and $B$, and can be written as $A ∩ B$.

<iframe scrolling="no" title="Copy of Sets Union and Intersection by how final" src="https://www.geogebra.org/material/iframe/id/nas3nnut" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>
- **Complement:** The complement of $A$, frequently denoted by $\bar{A}$, is the set of all elements which do not belong to $A$. In making this definition we assume that all elements we are thinking about belong to some larger set $U$, which we call the **universal** set.
- **Difference:** The difference of two sets $A$ and $B$, denoted as $A$ \ $B$ or $A - B$, is the set that contains all the elements that are in $A$ but not in $B$.
- **Cartesian Product:** The Cartesian product of two sets $A$ and $B$ denoted as $A × B$, is the set of all possible ordered pairs $(a, b)$ where a is in $A$ and $b$ is in $B$.

Sets are used in probability theory to represent events. The union of two events represents the event that either one or both occur, the intersection represents the event that both occur, and the complement represents the event that an event does not occur. Set operations, along with probability rules, enable us to calculate probabilities and analyze relationships between events.

<iframe scrolling="no" title="Copy of I learn Sets- Practice with Two Sets test 1" src="https://www.geogebra.org/material/iframe/id/je66pnv3" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

---

## Terms Related to Probability

- **Random Experiment:-** An experiment with a known set of possible outcomes is called a random experiment if it cannot be predicted in advance which specific outcome will occur on a given execution of the experiment. Random experiments include things like coin tosses, die rolls, and card draws from a deck.
- **Outcome:-** The result of any random experiment is called an outcome. Suppose you tossed a coin and got head$(H)$ as the upper surface. So, tossing a coin is a random experiment that results in an outcome ‘head’.
- **Sample Space:-** It is a set of all the possible outcomes for a random experiment. **For example -** Obtaining a head or a tail on the tossing of a coin is possible. Thus, $S$={H, T}: the Head and Tail are the sample space for tossing a coin. Similarly, on rolling a die, we can get either of the following numbers - 1, 2, 3, 4, 5, 6. Thus, S={1, 2, 3, 4, 5, 6} are the sample space for rolling a die.
- **Equally Likely Outcomes:-** Events with the same theoretical probability (or likelihood) of occurring are referred to as equally likely events. **For example**, the relative occurrences of Head and Tail on tossing a coin for a very large number of tosses are equal. So, Head and Tail are equally likely outcomes that make the tossing of a coin fair and unbiased if it's to decide between two options.
- **Event:-** In the case of a random experiment, an event is a set of possible outcomes at a specified condition. **Example -** On rolling of a die, 4 is not obtained. This event is the random experiment that is rolling of a die whose result is not 4. Thus, this event has 5 possible outcomes that are 1, 2, 3, 5, and 6. Suppose it's mentioned that the event F is equal to obtaining a black card while drawing a card from a deck of 52 cards. In this case, event F has 26 possible outcomes because there are 26 black cards, a total that is 13 spades and 13 clubs.


## Probability Formula

Look at the example of rolling a six faced die. The possible outcomes in this experiment are 1,2,3,4,5,6, so the sample space is the set {1,2,3,4,5,6}. The ‘event’ of ‘getting a 6’ is the subset {6}. We represent this in the following diagram.
<!DOCTYPE html>
<html>
<head>
<title>Responsive Image</title>
<style>
.responsive-image {
max-width: 100%;
height: auto;
}
</style>
</head>
<body>
<img class="responsive-image" src="https://drive.google.com/uc?export=view&id=1a3jBeYjRT1KMaZdFHCiRf2miZQvA_5Ew" alt="Embedded Image">
</body>
</html>

There are six possibilities in the sample space and only one of these corresponds to getting a 6, so the probability of getting a 6 when you roll a die is $\frac{1}{6}$ .
We say that the probability of an event $A$ occuring is

## $P(A)=\frac{Number\,of \,elements\, in\, A}{Total \,number\, of\, elements\, in\, the\, sample \,space}$

### Example:-

A card is selected at random from a pack of 52 cards. Let $A$ = ‘the card is a heart’ and $B$ = ‘the card is an ace’.
Find $P(A)$, $P(B)$?

### Solution

$P(A)$ =  $\frac{13}{52}$ since there are 13 hearts in the pack.
$P(B)$ =  $\frac{4}{52}$ since there are 4 aces in the pack.
To calculate the probability of an event, we simply need to find out the total number of possible outcomes of an experiment and the number of outcomes which correspond to the given event.

### Exercise ...

$Question:-$Danish Abdullah is playing a card game with a standard 52-card deck. He’s hoping for a club or a face card on his first draw. What is the probability that he draws a club or a face card on his first draw?
$Answer:-$
<iframe scrolling="no" title="Example 2" src="https://www.geogebra.org/material/iframe/id/EDsHcC4k" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

## Law's of Probability

- $P(A ∪ B) = P(A) + P(B) - P(A ∩ B)$.
- $P(A\,only) = P(A)-P(A ∩ B)$.
- $P(B,only) = P(B)-P(A ∩ B)$
- 
### $De\,Morgan's\,law$

    * $P(\bar{A ∪ B})= P(\bar{A} ∩\bar{B})$
    * $P(\bar{A ∩ B})=P(\bar{A}∪\bar{B})$

Probability Venn Diagram with proportionally-sized regions.
**Control $P(A), P(B)$ and $P(A∩B)$**
<iframe scrolling="no" title="Probability Venn Diagram" src="https://www.geogebra.org/material/iframe/id/Bjw5nAvK" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

---

## Events in Probability

Assume that event $(E)$ can occur in $(r)$ favorable ways and let $(n)$ be the total number of ways. Then the probability of an event or success being achieved is highlighted as;

#### $P(E)= \frac{r}{n}$

The probability of an event not occurring or being known as a failure is set out as follows:

#### $P(\bar{E})=\frac{(n-r)}{n}=1-\frac{r}{n}$

Where $P(\bar{E})$ represents that the event $(E)$ will not take place.

So, now we can say;

#### $P(E)+P(\bar{E})=\frac{r}{n}+1-\frac{r}{n}$

#### $P(E)+P(\bar{E})=1$

This means that the sum of all the probabilities for any random event or test is equal to $1$.

## Types of Event

1. **Simple Event:** A simple event is an event that represents a single outcome or elementary event in an experiment. For example, rolling a specific number on a fair die, such as rolling a 3.
2. **Compound Event:** A compound event is an event that consists of two or more simple events. It involves multiple outcomes or combinations of outcomes. For example, rolling an even number or flipping a coin and getting heads.
3. **Independent Events:** Independent events are events where the occurrence of one event does not affect the probability of the other event. The outcome of one event has no influence on the outcome of the other. For example, flipping a coin and rolling a die are independent events.

- For indpendent event:- $P(A ∩ B)= P(A).P(B)$

5. **Dependent Events:** Dependent events are events where the occurrence of one event does affect the probability of the other event. The outcome of one event impacts the outcome of the other. For example, drawing two cards from a deck without replacement, where the probability of the second card depends on the outcome of the first card.
6. **Mutually Exclusive Events:** Mutually exclusive events are events that cannot occur simultaneously. If one event happens, the other event cannot happen at the same time. For example, rolling an even number and rolling an odd number are mutually exclusive events when using a fair six-sided die.
<style>
.responsive-image {
max-width: 100%;
height: auto;
}
</style>

<img class="responsive-image" src="https://drive.google.com/uc?id=1vN8Ve0H7-Pfkdxiq0SdTyNqYYhjbFOpP" alt="Embedded Image">

- $P(A ∩ B)=0$

8. **Exhaustive Events:** Exhaustive events are events that cover all possible outcomes in an experiment. Together, they encompass the entire sample space, ensuring that at least one of the events must occur. For example, when rolling a fair six-sided die, the events of rolling an even number or rolling an odd number are exhaustive events.

### Exercise ...

$Question:-$Students at **Jamia Hamdard** receive an achievement award for either performing community service or making the honor roll. The school has 500 students and 180 of them received the award. There were 125 students who performed community service and 75 students who made the honor roll. What is the probability that a randomly chosen student at **Jamia Hamdard** performed community service and made the honor roll?
$Answer:-$
<iframe scrolling="no" title="Example 4" src="https://www.geogebra.org/material/iframe/id/RXUGRyya" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

# Conditional Probability

Conditional probability is a concept in probability theory that measures the probability of an event occurring given that another event has already occurred. It is denoted as P(A|B), which represents the probability of event A happening given that event B has occurred.

The formula for conditional probability is:

### $P(A|B) = \frac{P(A ∩ B)}{P(B)}$

Where:

- $P(A|B)$ is the conditional probability of event $A$ given event $B$.
- $P(A ∩ B)$ represents the probability of both events $A$ and $B$ occurring simultaneously.
- $P(B)$ is the probability of event $B$ occurring.

In simpler terms, conditional probability allows us to update the probability of an event based on new information or conditions. It measures the likelihood of an event happening within a specific context or condition.
**Note:-** For indpendent event:- $P(A|B)= P(A)$

**For example**, let's say we have two events: $A$ and $B$. The probability of event $A$ occurring is $0.6$, and the probability of event $B$ occurring is $0.3$ . If we want to find the probability of event $A$ occurring given that event $B$ has already occurred, we need to use the formula above.

Assuming there is some relationship between $A$ and $B$, we would need additional information to determine $P(A ∩ B)$, which represents the probability of both $A$ and $B$ happening together. Once we have that value, we can divide it by $P(B)$ to calculate the conditional probability $P(A|B)$.

Conditional probability is a fundamental concept in probability theory and has applications in various fields, including statistics, data analysis, machine learning, and decision-making. It helps us reason about uncertain events and make predictions based on available information.
**Geometrical Understanding**

<iframe scrolling="no" title="conditional probability " src="https://www.geogebra.org/material/iframe/id/asbbx8my" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

### Exercise ...

<iframe scrolling="no" title=" Conditional Probability question" src="https://www.geogebra.org/material/iframe/id/fyecncmu" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

# Total Probability Theorem

The Total Probability Theorem is a concept in probability theory that helps us calculate the probability of an event when we have information about its occurrence under different conditions.

Imagine you have an event, let's call it "$A$," and there are several possible scenarios or conditions, let's call them "$B1$," "$B2$," .......... "$Bn$". and so on. These scenarios are mutually exclusive, meaning that only one of them can happen. The Total Probability Theorem helps us find the overall probability of event A by considering the probabilities of A happening in each scenario, and then combining them.
<style>
.responsive-image {
max-width: 100%;
height: auto;
}
</style>

<img class="responsive-image" src="https://drive.google.com/uc?id=1rzDM8w5I7Qijr8lyKJ8Jss9NMasrgyKn" alt="Embedded Image">

In simpler words, the theorem says that to find the probability of event $A$, we should look at each scenario or condition $(B1, B2, etc.)$, consider how likely event $A$ is in each scenario, and then multiply that probability by the probability of the corresponding scenario occurring. We do this for all scenarios and then add up the results.

By using the Total Probability Theorem, we can handle situations where we don't know the direct probability of event A but have information about its occurrence under different conditions. It allows us to calculate the overall probability of A by considering all possible scenarios or conditions.

- $P(A)= P(B1 ∩ A)+P(B2 ∩ A)+P(B3 ∩ A)+.....+P(B8 ∩ A)$


# Baye's Theorem

Bayes' theorem is a fundamental concept in probability theory and statistics that allows us to update the probability of an event based on new evidence or information. It is named after the Reverend Thomas Bayes, an 18th-century British mathematician and clergyman.

Mathematically, Bayes' theorem is stated as:

### $P(A \mid B)=\frac{P(B \mid A) P(A)}{P(B)}$

Where:

$P(A|B)$ is the conditional probability of event $A$ given event $B$.
$P(B|A)$ is the conditional probability of event $B$ given event $A$.
$P(A)$ and $P(B)$ are the probabilities of events $A$ and $B$, respectively.

In simpler terms, Bayes' theorem allows us to calculate the probability of event $A$ occurring given that event $B$ has already occurred, by taking into account the probability of event $B$ given event $A$ and the prior probabilities of events $A$ and $B$.

The numerator of the formula, ${P(B|A)}\times { P(A)}$, represents the joint probability of both events $A$ and $B$ occurring simultaneously. The denominator, $P(B)$, is the probability of event $B$ occurring, regardless of event $A$.

Bayes' theorem is particularly useful in situations where we have prior knowledge or beliefs about the probabilities of certain events, and we want to update those probabilities based on new evidence. It forms the foundation of Bayesian statistics, which is a statistical approach that incorporates prior knowledge and evidence to make inferences and predictions.

Bayes' theorem has applications in various fields, including medical diagnosis, spam filtering, machine learning, and artificial intelligence. It provides a framework for reasoning under uncertainty and updating probabilities as new information becomes available.

**Geometrical Understanding**
Imagine you have two events,$A$ and $B$, and you are interested in calculating the probability of event $A$ given that event $B$ has occurred, denoted as $P(A|B)$. Bayes' theorem provides a way to update our prior belief about the probability of $A$ in light of new evidence from event $B$.

Geometrically, we can represent the probability space as a rectangle, with its area representing the total probability of $1$.
Let's denote this rectangle as the entire space $Ω$.

Now, within this probability space, let's focus on a smaller subset that represents event $B$. This subset will have an area proportional to the probability of event $B$, denoted as $P(B)$. So, $B$ is a region within the larger rectangle $Ω$.

Next, we consider the conditional probability $P(A|B)$, which is the probability of event $A$ occurring given that event $B$ has occurred. In terms of the geometric representation, we look at the region where both $A$ and $B$ occur, denoted as $A ∩ B$. The area of $A ∩ B$ within the region $B$ represents the probability of both $A$ and $B$ occurring, $P(A ∩ B)$.

Now, let's apply Bayes' theorem:

$P(A|B) = (P(B|A) * P(A)) / P(B)$

In geometric terms, $P(B|A)$ represents the probability of event $B$ occurring given that event $A$ has occurred. This is like looking at the overlap of $A$ and $B$ within the region $A$, denoted as $B ∩ A$.

$P(A)$ represents the prior probability of $A$, which is the overall probability of event $A$ occurring without considering event $B$. In the geometric representation, this is the area of the region $A$ within the entire space $Ω$.

Finally, $P(B)$ is the total probability of event $B$ occurring, which is the sum of the probabilities of $B$ occurring under different conditions. Geometrically, this is the combined area of $B$ and $A$ within $Ω$.

If you want to dive deeper into this topic, please check out this video:-

<iframe width="560" height="315" src="https://www.youtube.com/embed/HZGCoVF3YvM?controls=0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

**Example:-** If a person tests positive for a disease, what is the probability that he or she is actually infected?

The user can enter the following quantities by using the input boxes or the sliders:

- **Incidence** is the percentage of the general population that is infected.
- **False positive** rate is the probability that a person who is not infected will test positive for the disease.
- **False negative** rate is the probability that a person who is infected will test negative for the disease.

The pie chart shows the conditional probability that a person is infected given that he or she tests positive for the disease.

<iframe scrolling="no" title="Exploring Bayes' Theorem" src="https://www.geogebra.org/material/iframe/id/HsSCSPW5" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

# Random Variables

In probability theory, a random variable is a mathematical function that maps outcomes of a random experiment to numerical values. It represents an uncertain quantity whose value is determined by the outcome of a random event or process. Random variables provide a way to quantify the uncertainty associated with different outcomes and are a fundamental concept in probability and statistics.

Formally, a random variable is denoted by a capital letter $(e.g., X, Y)$ and can take on various values based on the possible outcomes of the underlying random experiment. The set of all possible values that a random variable can take is called its "sample space."

There are two main types of random variables:

1. **Discrete Random Variable:-** A random variable is called discrete if it can only take on a countable number of distinct values. The probability distribution of a discrete random variable describes the probabilities associated with each possible value it can take. The probabilities must sum up to 1.

Example of a discrete random variable: The number rolled on a fair six-sided die.

2. **Continuous Random Variable:-** A random variable is called continuous if it can take on any value within a certain range or interval. Continuous random variables are associated with probability density functions (PDFs) instead of probability mass functions (PMFs).

Example of a continuous random variable: The height of a person selected at random from a population.

Random variables are essential for quantifying uncertainties and making predictions in various fields, including finance, engineering, economics, and more. They serve as a bridge between theoretical probability concepts and practical applications in real-world situations.

# Distribution

Distribution refers to the way in which the values of a random variable are spread or distributed across a set of possible outcomes. It provides a description of the likelihood of various possible values occurring and the associated probabilities. Distributions can be characterized by their shape, center, and spread.

There are various types of distributions, and they can be classified as either discrete or continuous:

**Discrete Distribution:** A discrete distribution is applicable to discrete random variables, which take on specific isolated values with gaps between them. The probability mass function (PMF) describes the probabilities of different outcomes. Examples of discrete distributions include the Bernoulli distribution, Binomial distribution, and Poisson distribution.

**Continuous Distribution:** A continuous distribution is applicable to continuous random variables, which can take any value within a range or interval. The probability density function (PDF) characterizes the probabilities of intervals of values. Examples of continuous distributions include the Normal distribution, Uniform distribution, and Exponential distribution.

- **Normal Distribution:** The Normal distribution, also known as the Gaussian distribution, is one of the most common and important probability distributions in statistics. It is a continuous distribution characterized by a symmetric bell-shaped curve.


# Discrete Probability Distribution

When dealing with **discrete random variables**, we use probability mass functions (PMFs) to describe their probability distributions. A probability mass function assigns probabilities to specific outcomes or values that the random variable can take.

Let's consider an example with a discrete random variable $X$. The probability mass function for $X$, denoted as $P(X = n)$, gives the probability of $X$ being equal to a particular value $n$. The PDF satisfies the following properties:

- Non-Negativity: $P(X = n) ≥ 0$ for all possible values of $n$.
- Summation: The sum of the probabilities for all possible values of $X$ is equal to 1: $Σ P(X = n) = 1$, where the summation is taken over all possible values of $X$.

For instance, let's say we have a fair six-sided die, and we are interested in the random variable X representing the outcome of rolling the die. The PMF for this random variable would be:
|$X$|1|2|3|4|5|6
| :------------ |:-------------:| -----:|
|**$P(X=n)$**|$\frac{1}{6}$|$\frac{1}{6}$|$\frac{1}{6}$|$\frac{1}{6}$|$\frac{1}{6}$|$\frac{1}{6}$

Here, each possible outcome has an equal probability of $\frac{1}{6}$, satisfying the properties of a probability mass function.

The PDF allows us to calculate the probabilities of specific events or outcomes for discrete random variables. By summing the probabilities associated with the desired outcomes, we can determine the probability of those events occurring.

**Question:-** The probability distribution function for random variable is:
|$X$|0|1|2|3|4|5|6
| :------------ |:-------------:| -----:|
|**$P(X=n)$**|$K$|$3K$|$5K$|$7K$|$9K$|$11K$|$13K$
then find,

1. $P(X<4)$
2. $P(3<X\leqslant6)$
3. $P(X\geqslant 5)$
+++**Solution:-** Since it is a PDF,
$\sum_{0}^{6}P(X=n)=1$
$\Rightarrow \, P(X=0)+P(X=1)+P(X=2)+P(X=3)+P(X=4)+P(X=5)+P(X=6)=1$
$\Rightarrow \,K+3K+5K+7K+9K+11K+13K=1$
$\Rightarrow \,49K=1$
$\Rightarrow\, K = \frac{1}{49}$

**1.**  $P(X<4)=P(X=0)+P(X=1)+P(X=2)+P(X=3)$
$\Rightarrow \, K+3K+5K+7K$
$\Rightarrow \, 16K= 16\times\frac{1}{49}=\frac{16}{49}$
**2.** $P(3<X\leqslant6)=P(X=4)+P(X=5)+P(X=6)$
$\Rightarrow \, 9K+11K+13K$
$\Rightarrow \, 33K=33\times\frac{1}{49}=\frac{33}{49}$
**3.** $P(X\geq 5)= P(X=5)+P(X=6)$
$\Rightarrow \, 11K+13K=24K=24\times\frac{1}{49}=\frac{24}{49}$
+++
$\,$
$\,$
$\,$
**Question:-** Find the probability distribution function (PDF) for the number of heads when a fair coin is tossed three times?
+++ **Solution:-**
When a fair coin is tossed three times, there are 8 possible outcomes:

- HHH
- HHT
- HTH
- HTT
- THH
- THT
- TTH
- TTT

The probability of getting heads (H) or tails (T) in each toss is $0.5$. Therefore, the probabilities for each outcome are:

$$
\begin{align*}
  P(\text{HHH}) &= (0.5) \times (0.5) \times (0.5) = 0.125 \\
  P(\text{HHT}) &= (0.5) \times (0.5) \times (0.5) = 0.125 \\
  P(\text{HTH}) &= (0.5) \times (0.5) \times (0.5) = 0.125 \\
  P(\text{HTT}) &= (0.5) \times (0.5) \times (0.5) = 0.125 \\
  P(\text{THH}) &= (0.5) \times (0.5) \times (0.5) = 0.125 \\
  P(\text{THT}) &= (0.5) \times (0.5) \times (0.5) = 0.125 \\
  P(\text{TTH}) &= (0.5) \times (0.5) \times (0.5) = 0.125 \\
  P(\text{TTT}) &= (0.5) \times (0.5) \times (0.5) = 0.125 \\
\end{align*}
$$

Now, let's calculate the probability of each possible number of heads:

| Number of heads ($X$) | Probability ($P(X)$) |
| :---: | :---: |
| 0 | 0.125 |
| 1 | 0.375 |
| 2 | 0.375 |
| 3 | 0.125 |


The probability distribution function (PDF) for the number of heads when a fair coin is tossed three times is shown in the table above.
+++
$\,$
$\,$
$\,$
**Question:-** A pair of dice is thrown three times then find the probability distribution function of doublets?
+++ **Solution:-**

To find the probability distribution function (PDF) of doublets when a pair of dice is thrown three times, we need to consider all the possible outcomes and their probabilities.

A doublet is when the two dice show the same number after being thrown. There are six possible doublets: $(1, 1)$, $(2, 2)$, $(3, 3)$, $(4, 4)$, $(5, 5)$, and $(6, 6)$.

The probability of getting a specific doublet in a single throw of a pair of dice is given by:

**$$
P(\text{Doublet}) = \text{Probability of rolling the first number} \times \text{Probability of rolling the second number} = \frac{1}{6} \times \frac{1}{6} = \frac{1}{36}
$$**

Since we are throwing the pair of dice three times, the probability of getting a specific doublet three times in a row is given by:

$$
P(3 \text{ Doublets}) = \left(\frac{1}{36}\right) \times \left(\frac{1}{36}\right) \times \left(\frac{1}{36}\right) = \frac{1}{46656}
$$

Now, let's calculate the probabilities for getting different numbers of doublets:

| Number of doublets ($X$) | Probability ($P(X)$) |
| :---: | :---: |
| 0 | $P(0 \text{ Doublet}) = (1 - P(\text{Doublet}))^3 = \left(1 - \frac{1}{36}\right)^3 \approx 0.9885$ |
| 1 | $P(1 \text{ Doublet}) = 3 \times P(\text{Doublet}) \times (1 - P(\text{Doublet}))^2 \approx 3 \times \frac{1}{36} \times \left(\frac{35}{36}\right)^2 \approx 0.1095$ |
| 2 | $P(2 \text{ Doublets}) = 3 \times P(\text{Doublet})^2 \times (1 - P(\text{Doublet})) \approx 3 \times \left(\frac{1}{36}\right)^2 \times \frac{35}{36} \approx 0.0029$ |
| 3 | $P(3 \text{ Doublets}) \approx \frac{1}{46656}$ |


The probability distribution function (PDF) for the number of doublets when a pair of dice is thrown three times is shown in the table below.

| Number of doublets ($X$) | Probability ($P(X)$) |
| :---: | :---: |
| 0 | 0.9885 |
| 1 | 0.1095 |
| 2 | 0.0029 |
| 3 | $\frac{1}{46656}$ |


+++
$\,$
$\,$
$\,$

# Expectation of a discrete random variable

The expectation of a discrete random variable $X$, often denoted as $E(X)$ or $\mu$, represents the average or mean value of the random variable's possible outcomes. Mathematically, for a discrete random variable $X$ that can take values $x_1, x_2, \ldots, x_n$ with corresponding probabilities $P(X=x_1), P(X=x_2), \ldots, P(X=x_n)$, the expectation is given by:

### $$
E(X) =Mean(\mu)= x_1 \cdot P(X=x_1) + x_2 \cdot P(X=x_2) + \ldots + x_n \cdot P(X=x_n)
$$

In simpler terms, you multiply each possible outcome by its probability and sum up these products to obtain the expectation.

Here's a step-by-step example to calculate the expectation of a discrete random variable:

Let's say we have a discrete random variable $X$ representing the outcome of rolling a fair six-sided die, and its possible values are $\{1, 2, 3, 4, 5, 6\}$, each with a probability of $\frac{1}{6}$.

$$
E(X) = (1 \cdot \frac{1}{6}) + (2 \cdot \frac{1}{6}) + (3 \cdot \frac{1}{6}) + (4 \cdot \frac{1}{6}) + (5 \cdot \frac{1}{6}) + (6 \cdot \frac{1}{6})
$$

$$
E(X) = \frac{1}{6} + \frac{2}{6} + \frac{3}{6} + \frac{4}{6} + \frac{5}{6} + \frac{6}{6}
$$

$$
E(X) = \frac{21}{6}
$$

$$
E(X) = 3.5
$$

So, the expectation of rolling a fair six-sided die is 3.5. This means that, on average, we can expect the outcome of the die roll to be around 3.5, even though 3.5 itself is not one of the possible outcomes of rolling a regular six-sided die.

**2. $E(X^2)$ (Expectation of $X^2$):**

$$
E(X^2) = \sum_{i=1}^{n} x_i^2 \cdot P(X=x_i)
$$

$E(X^2) = x_1^2 \cdot P(X=x_1) + x_2^2 \cdot P(X=x_2) + \ldots + x_n^2 \cdot P(X=x_n)$

$E(X^2)$ represents the average value of the squared outcomes of a discrete random variable $X$. It is used to calculate the variance $\text{Var}(X)$.

**3. $\text{Var}(X)$ (Variance of $X$):**

$$
\text{Var}(X) = E(X^2) - (E(X))^2
$$

$\text{Var}(X)$ measures the spread or dispersion of the random variable $X$ from its mean. It is the difference between the expectation of $X^2$ and the square of the expectation of $X$.

**4. $E(f(X))$ (Expectation of a Function of $X$):**

$$
E(f(X)) = \sum_{i=1}^{n} f(x_i) \cdot P(X=x_i)
$$

**$E(f(X)) = f(x_1) \cdot P(X=x_1) + f(x_2) \cdot P(X=x_2) + \ldots + f(x_n) \cdot P(X=x_n)$**

$E(f(X))$ is the average value of the function $f(X)$ applied to the possible outcomes of the random variable $X$. Expectation is a linear operator, meaning that it follows certain rules when dealing with functions and constants.

These formulas are fundamental in probability theory and statistics, playing a key role in various statistical measures and analyses.
$\,$
$\,$
$\,$
**Question:-** The PDF of random variable is given by:
|$X$|1|2|3|4|
| :------------ |:-------------:| -----:|
|**$P(X=n)$**|$\frac{1}{4}$|$\frac{1}{4}$|$\frac{1}{4}$|$\frac{1}{4}$
Find,

1. $E(X)$
2. $E(X^2)$
3. $Var(X)$
4. $E(2X+1)$
+++ **Solution:-**
**1.**  $E(X)=\sum_{n=1}^{4}P_{i}X_{i}\Rightarrow1\times\frac{1}{4}+2\times\frac{1}{4}+3\times\frac{1}{4}+4\times\frac{1}{4}$
$\,$
$\Rightarrow\frac{1}{4}\times(1+2+3+4)\Rightarrow\frac{1}{4}\times10\Rightarrow\frac{5}{2}$
$\,$
**2.**$E(X^2)=\sum_{i=1}^{n} x_i^2 \cdot P_{i}$
$\Rightarrow\,(1)^2\times\frac{1}{4}+(2)^2\times\frac{1}{4}+(3)^2\times\frac{1}{4}+(4)^2\times\frac{1}{4}$
$\Rightarrow\,\frac{1}{4}+\frac{4}{4}+\frac{9}{4}+\frac{16}{4}\,\Rightarrow\,\frac{1}{4}+\frac{1}{1}+\frac{9}{4}+\frac{4}{1}\Rightarrow\,\frac{15}{2}$
$\,$
**3.** $Var(X)=E(X^2) - (E(X))^2$
$\Rightarrow\,\frac{15}{2}-(\frac{5}{2})^2\Rightarrow\,\frac{5}{4}$
$\,$
**4.** $E(2X+1)=\sum_{i=1}^{n} (2X_{i}+1)^2 \cdot P_{i}$
$\Rightarrow\,(2\times1+1)\cdot\frac{1}{4}+(2\times2+1)\cdot\frac{1}{4}+(2\times3+1)\cdot\frac{1}{4}+(2\times4+1)\cdot\frac{1}{4}$
$\Rightarrow\,\frac{3}{4}+\frac{5}{4}+\frac{7}{4}+\frac{9}{4}\Rightarrow\,6$
+++
$\,$
$\,$
$\,$

## Moment Generating Function (MGF) of Discrete Random Variable

The Moment Generating Function (MGF) of a discrete random variable is a mathematical function that uniquely characterizes the random variable and provides a way to find its moments. It is defined as the expected value of the exponential function raised to the power of the random variable multiplied by a constant $t$. For a discrete random variable $X$ with probability mass function (PMF) $P(X = x)$, the MGF is given by:

$$
M_X(t) = E[e^{tX}] = \sum_{x} e^{tx} \cdot P(X = x)
$$

where the summation is taken over all possible values of the random variable $X$.

The MGF has several important properties:

1. The MGF is defined for all values of $t$ in an interval containing zero.
2. The $n$th moment of the random variable can be obtained by differentiating the MGF $n$ times with respect to $t$ and setting $t = 0$. Specifically, the $n$th moment is given by $E[X^n] = M_X^{(n)}(0)$, where $M_X^{(n)}(0)$ represents the $n$th derivative of $M_X(t)$ evaluated at $t = 0$.
3. If the MGF exists and is finite in a neighborhood of zero, then it uniquely determines the probability distribution of the random variable $X$.

The MGF is particularly useful in finding moments of a random variable, especially in cases where finding the moments directly from the PMF may be difficult or tedious. Additionally, the MGF is applicable to both discrete and continuous random variables, providing a unified approach to handling various types of distributions. However, not all random variables have a valid MGF for all values of $t$, especially when the distribution is heavy-tailed or lacks certain moments.
$\,$
$\,$
$\,$
**Question:-** Let 'X' be discrete random variable with PDF:
|$X$|1|2|3|4|5|6
| :------------ |:-------------:| -----:|
|**$P(X=n)$**|$\frac{1}{6}$|$\frac{1}{6}$|$\frac{1}{6}$|$\frac{1}{6}$|$\frac{1}{6}$|$\frac{1}{6}$
then, find the MGF?
+++  **Hint:-**
$M(t) = E[e^{tX}]$
+++
$\,$
$\,$
$\,$

# Binomial Distribution

The binomial distribution is a discrete probability distribution that describes the number of successes in a fixed number of independent Bernoulli trials (experiments) with the same probability of success, denoted by $p$. Each trial can have only two possible outcomes, usually labeled as "success" (probability $p$) and "failure" (probability $1-p$).

Let's denote the random variable that follows a binomial distribution as $X$. The probability mass function (PMF) of the binomial distribution is given by:

### $$
P(X = k) =\, ^{n}\textrm{C}_{k}\cdot p^k \cdot (1-p)^{n-k},
$$

where:

- $P(X = k)$ is the probability that there are $k$ successes in $n$ trials.
- $n$ is the number of trials (fixed and known in advance).
- $k$ is the number of successes (the value we want to find the probability for).
- $p$ is the probability of success on each individual trial.
- $^{n}\textrm{C}_{k}$ is the binomial coefficient, also known as "n choose k," which is the number of ways to choose $k$ successes from $n$ trials, given by $^{n}\textrm{C}_{k} = \frac{n!}{k!(n-k)!}$.

<iframe scrolling="no" title="binomial distribution" src="https://www.geogebra.org/material/iframe/id/zejjwwc7" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

**Note:-** Some times we use    $\,\,\,q=1-p$
The mean (expected value) and variance of a binomial distribution are given by:

$$
E[X] =Mean(\mu)=n \cdot p
$$

$$
Var[X] = n \cdot p \cdot (1-p)=n\cdot p\cdot q
$$

Key Properties of the Binomial Distribution:

1. Each trial is independent of others.
2. There are only two outcomes (success or failure) for each trial.
3. The probability of success ($p$) is constant for all trials.
4. The random variable $X$ represents the count of successes in $n$ trials.
5. The binomial distribution is symmetric when $p = 0.5$, and it is positively skewed for $p < 0.5$ and negatively skewed for $p > 0.5$.
6. As $n$ increases, the binomial distribution approaches the normal distribution if $np$ and $n(1-p)$ are sufficiently large.

The binomial distribution is commonly used in various fields, such as statistics, genetics, quality control, and polling, where we are interested in the number of successes in a fixed number of trials with a known probability of success.
$\,$
**Question:-** A coin is tossed 5-times, the, find the probability$\rightarrow$

1. Getting exactly 3 heads.
2. Getting at least 3 heads.
3. Getting at most 4 heads.
+++ **Solution:-**
$n=5$
$p=\frac{1}{2}$
**1.** $P(X=3)=^{n}\textrm{C}_{k}\cdot p^k \cdot (1-p)^{n-k}$
$\Rightarrow \,^{5}\textrm{C}_{3}\cdot \frac{1}{2}^3 \cdot (1-\frac{1}{2})^{5-3}$
$\Rightarrow\,\frac{5}{16}$
$\,$
**2.** $P(X\geq 3)=P(X=3)+P(X=4)+P(X=5)$
$\Rightarrow \,^{5}\textrm{C}_{3}\cdot \frac{1}{2}^3 \cdot (1-\frac{1}{2})^{5-3}+\,^{5}\textrm{C}_{4}\cdot \frac{1}{2}^4 \cdot (1-\frac{1}{2})^{5-4}+\,^{5}\textrm{C}_{5}\cdot \frac{1}{2}^5 \cdot (1-\frac{1}{2})^{5-5}$
$\Rightarrow\, \frac{1}{2}$
+++
$\,$
$\,$
**Exersise:-** A multiple-choice test has 8 problems. Each problem has 4 answer choices, and only 1 correct answer. You haven’t studied at all, and decide that your only chance to earn at least some points is to guess. Is this situation an example of a binomial distribution? Create a probability distribution for the number of problems you could answer correctly by guessing. What is the probability that your grade on the test will be 80% or greater?

<iframe scrolling="no" title="normal distribution question" src="https://www.geogebra.org/material/iframe/id/na9yhyre" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

# Poisson Distribution

The Poisson distribution is a discrete probability distribution that models the number of events that occur in a fixed interval of time or space. It is used to describe rare events with a known average rate of occurrence ($\lambda$).

The probability mass function (PMF) of the Poisson distribution is given by:

$$
P(X = k) = \frac{e^{-\lambda} \cdot \lambda^k}{k!},
$$

where:

- $X$ is the random variable representing the number of events.
- $k$ is the number of events ($0, 1, 2, \ldots$).
- $\lambda$ is the average rate of occurrence of events in the given interval.

The mean (expected value) and variance of the Poisson distribution are both equal to $\lambda$.

**Example:**

- Let Lambda be the mean of people making line at a random moment.
- Select the number of people making line at that random moment.
- What is the probability of X persons making line at that moment?.
**Play with the sliders and find out the answer**

<iframe scrolling="no" title="Poisson Distribution" src="https://www.geogebra.org/material/iframe/id/kpwgwgcu" width="100%" height="100%" style="border:0px; aspect-ratio:16/9;">
</iframe>

The Poisson distribution is commonly used in various fields, such as modeling rare events in insurance, telecommunications, and queuing systems, where events occur randomly and independently at a constant average rate.

**Question:**

The number of customers arriving at a coffee shop follows a Poisson distribution with an average rate of 5 customers per hour.

a) What is the probability that exactly 3 customers arrive in the next hour?

b) What is the probability that more than 7 customers arrive in the next two hours?

+++ **Solution:**

a) To find the probability that exactly 3 customers arrive in the next hour, we will use the Poisson probability formula:

For a Poisson distribution with rate $\lambda$ and a random variable $X$ representing the number of events, the probability of getting exactly $x$ events is given by:

$$
P(X = x) = \frac{{e^{-\lambda} \cdot \lambda^x}}{{x!}}
$$

where $e$ is the base of the natural logarithm (approximately 2.71828).

In this case, $\lambda = 5$ (average rate of customers per hour) and $x = 3$ (exactly 3 customers).

$$
P(X = 3) = \frac{{e^{-5} \cdot 5^3}}{{3!}}
$$

$$
P(X = 3) = \frac{{e^{-5} \cdot 125}}{{6}}
$$

To find the numerical value of $P(X = 3)$, you can use a calculator or software to compute the expression. The approximate value is:

$$
P(X = 3) \approx 0.140373
$$

b) To find the probability that more than 7 customers arrive in the next two hours, we need to consider the cumulative probability. The number of customers arriving in two hours follows a Poisson distribution with rate $\lambda' = 2 \cdot \lambda = 2 \cdot 5 = 10$.

Let $Y$ be the number of customers arriving in the next two hours. We want to find $P(Y > 7)$, which can be calculated as follows:

$$
P(Y > 7) = 1 - P(Y \leq 7)
$$

To find $P(Y \leq 7)$, we sum the probabilities of getting 0, 1, 2, ..., 7 customers in the next two hours using the Poisson probability formula:

$$
P(Y \leq 7) = \sum_{x=0}^{7} \frac{{e^{-10} \cdot 10^x}}{{x!}}
$$

Once again, you can use a calculator or software to find the numerical value of $P(Y \leq 7)$. The approximate value is:

$$
P(Y \leq 7) \approx 0.967206
$$

Now, calculate $P(Y > 7)$:

$$
P(Y > 7) = 1 - 0.967206
$$

$$
P(Y > 7) \approx 0.032794
$$

Therefore, the probability that more than 7 customers arrive in the next two hours is approximately 0.032794, or 3.28\%.
+++

