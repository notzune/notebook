below is a formula sheet I wrote in python, each formula can be called and used as a calculator.

---
### Basic Probability

- **Probability** of an event E is `P(E)`, where 0 ≤ P(E) ≤ 1.
- **Sample Space (S)**: The set of all possible outcomes.
- **Event**: A subset of the sample space.
- **Complementary Event**: `P(A') = 1 - P(A)`.
- **Mutually Exclusive Events**: Cannot occur at the same time; `P(A ∩ B) = 0`.
- **Independent Events**: Occurrence of one does not affect the other; `P(A ∩ B) = P(A)P(B)`.

### Probability Distributions

- **Discrete Random Variables**: Take on countable values.
- **Continuous Random Variables**: Take on values over a continuum.
- **Binomial Distribution**: `P(X = k) = (n choose k) p^k (1-p)^(n-k)`, where `n` is the number of trials, `p` is the probability of success, and `k` is the number of successes.
- **Normal Distribution**: Described by its mean (μ) and standard deviation (σ), with PDF `f(x) = (1/(σ√(2π))) e^(-(x-μ)²/(2σ²))`.
- **Poisson Distribution**: For a given λ, `P(X = k) = (e^(-λ) λ^k)/k!`, where λ is the average number of events in an interval.

### Descriptive Statistics

- **Mean (μ or x̄)**: Average value.
- **Median**: Middle value when data is ordered.
- **Mode**: Most frequently occurring value.
- **Variance (σ² or s²)**: Average of the squared differences from the mean.
- **Standard Deviation (σ or s)**: Square root of the variance.
- **Skewness**: Measure of asymmetry.
- **Kurtosis**: Measure of the "tailedness" of the probability distribution.

### Inferential Statistics

- **Central Limit Theorem (CLT)**: With a large enough sample size, the sampling distribution of the sample mean will be normally distributed, regardless of the shape of the population distribution.
- **Confidence Intervals**: Range where a population parameter lies with a certain probability.
- **Hypothesis Testing**: Procedure to decide if a hypothesis about a population parameter should be rejected or not.
- **p-value**: The probability of observing a test statistic as extreme as, or more extreme than, the value observed, under the assumption that the null hypothesis is true.

### Correlation and Regression

- **Correlation Coefficient (ρ or r)**: Measures the strength and direction of linear relationship between two variables.
- **Linear Regression**: Models the relationship between two variables by fitting a linear equation to observed data.
- **Regression Coefficient (β)**: Describes the change in the dependent variable for a one-unit change in the independent variable.

### Special Topics

- **Bayes' Theorem**: `P(A|B) = P(B|A)P(A) / P(B)`, used to update the probability estimate for A as more information becomes available.
- **Chebyshev's Inequality**: For any distribution with a finite standard deviation, no more than 1/k² of the distribution's values can be more than k standard deviations away from the mean.
- **Law of Large Numbers**: As a sample size grows, its mean gets closer to the average of the whole population.

### Important Formulas and Concepts to Remember

- **Combination**: `n choose k = n! / (k!(n-k)!)`, the number of ways to choose k elements from a set of n elements without regard to the order of selection.
- **Permutation**: `P(n, k) = n! / (n-k)!`, the number of ways to arrange k elements out of n elements.
- **Z-Score**: `(X - μ) / σ`, represents the number of standard deviations an element X is from the mean μ.
- **Law of Total Probability**: If {B₁, B₂, ..., Bₙ} is a partition of the sample space S, then for any event A, `P(A) = Σ P(A ∩ Bᵢ)`.
- **Marginal Probability**: The probability of an event irrespective of the outcome of another variable.
- **Joint Probability**: `P(A and B)`, the probability of two events occurring together.
- **Conditional Probability**: `P(A|B)`, the probability of A given B has occurred.

---

```python
import math
import numpy as np
import scipy.stats as stats
from scipy.stats import norm, poisson


def permutations(n, r):
    """
    Calculate the number of permutations of choosing r items from n items.

    Parameters:
    n (int): The total number of items.
    r (int): The number of items to choose.

    Returns:
    int: The number of permutations.
    """
    return math.factorial(n) / math.factorial(n - r)


def combinations(n, r):
    """
    Calculate the number of combinations of choosing r items from n items.

    Parameters:
    n (int): The total number of items.
    r (int): The number of items to choose.

    Returns:
    int: The number of combinations.
    """
    return math.factorial(n) / (math.factorial(r) * math.factorial(n - r))


def binomial_probability(k, n, p):
    """
    Calculate the probability of k successes in n trials with success probability p in each trial.

    Parameters:
    k (int): Number of successes.
    n (int): Number of trials.
    p (float): Probability of success in each trial.

    Returns:
    float: Probability of getting exactly k successes.
    """
    return combinations(n, k) * (p ** k) * ((1 - p) ** (n - k))


def normal_distribution_pdf(x, mean, std_dev):
    """
    Calculate the probability density of the normal distribution at a point x.

    Parameters:
    x (float): Point at which to evaluate the PDF.
    mean (float): Mean of the distribution.
    std_dev (float): Standard deviation of the distribution.

    Returns:
    float: The probability density at point x.
    """
    return (1 / (std_dev * math.sqrt(2 * math.pi))) * math.exp(-0.5 * ((x - mean) / std_dev) ** 2)


def normal_distribution_cdf(x, mean, std_dev):
    """
    Calculate the cumulative distribution function (CDF) of the normal distribution at a point x.

    Parameters:
    x (float): Point at which to evaluate the CDF.
    mean (float): Mean of the distribution.
    std_dev (float): Standard deviation of the distribution.

    Returns:
    float: The cumulative probability up to point x.
    """
    return stats.norm.cdf(x, mean, std_dev)


def poisson_probability(k, lambda_):
    """
    Calculate the probability of k events in a Poisson distribution with a given lambda (average rate of success).

    Parameters:
    k (int): Number of events.
    lambda_ (float): The average number of events in an interval.

    Returns:
    float: Probability of observing k events.
    """
    return (lambda_ ** k) * math.exp(-lambda_) / math.factorial(k)


def exponential_distribution_pdf(x, lambda_):
    """
    Calculate the probability density of the exponential distribution at a point x.

    Parameters:
    x (float): Point at which to evaluate the PDF.
    lambda_ (float): Rate parameter (inverse of the mean).

    Returns:
    float: The probability density at point x.
    """
    return lambda_ * math.exp(-lambda_ * x)


def exponential_distribution_cdf(x, lambda_):
    """
    Calculate the cumulative distribution function (CDF) of the exponential distribution at a point x.

    Parameters:
    x (float): Point at which to evaluate the CDF.
    lambda_ (float): Rate parameter (inverse of the mean).

    Returns:
    float: The cumulative probability up to point x.
    """
    return 1 - math.exp(-lambda_ * x)


def calculate_z_score(x, mean, std_dev):
    """
    Calculate the z-score of a value x in a distribution.

    Parameters:
    x (float): The value for which the z-score is calculated.
    mean (float): Mean of the distribution.
    std_dev (float): Standard deviation of the distribution.

    Returns:
    float: The z-score of x.
    """
    return (x - mean) / std_dev


def confidence_interval_mean(sample_mean, std_dev, sample_size, confidence_level):
    """
    Calculate the confidence interval for a population mean,
    given a sample mean, standard deviation, sample size, and confidence level.

    Parameters:
    sample_mean (float): The mean of the sample.
    std_dev (float): The standard deviation of the sample.
    sample_size (int): The size of the sample.
    confidence_level (float): The confidence level (e.g., 0.95 for 95% confidence).

    Returns:
    tuple: A tuple containing the lower and upper bounds of the confidence interval.
    """
    alpha = 1 - confidence_level
    z = stats.norm.ppf(1 - alpha / 2)
    margin_error = z * (std_dev / math.sqrt(sample_size))
    return sample_mean - margin_error, sample_mean + margin_error


def probability_of_drawing_cards(num_cards, desired_cards, deck_size=52):
    """
    Calculate the probability of drawing a certain number of desired cards from a deck.

    Parameters:
    num_cards (int): Number of cards to draw.
    desired_cards (int): Number of desired cards in the deck.
    deck_size (int): Total number of cards in the deck. Defaults to 52 for a standard deck.

    Returns:
    float: The probability of drawing the desired cards.
    """
    total_ways_to_draw = math.comb(deck_size, num_cards)
    ways_to_draw_desired = math.comb(desired_cards, num_cards)
    return ways_to_draw_desired / total_ways_to_draw


def probability_with_replacement(successful_outcomes, total_outcomes, num_trials):
    """
    Calculate the probability of a certain event happening over a number of trials with replacement.

    Parameters:
    successful_outcomes (int): Number of successful outcomes in each trial.
    total_outcomes (int): Total number of possible outcomes in each trial.
    num_trials (int): Number of trials.

    Returns:
    float: The probability of the event happening in the given number of trials.
    """
    single_trial_probability = successful_outcomes / total_outcomes
    return single_trial_probability ** num_trials


def probability_without_replacement(successful_outcomes, total_outcomes, num_trials):
    """
    Calculate the probability of a certain event happening over a number of trials without replacement.

    Parameters:
    successful_outcomes (int): Number of successful outcomes in each trial.
    total_outcomes (int): Total number of possible outcomes in each trial.
    num_trials (int): Number of trials.

    Returns:
    float: The probability of the event happening in the given number of trials.
    """
    probability = 1
    for i in range(num_trials):
        probability *= (successful_outcomes - i) / (total_outcomes - i)
    return probability


def hypergeometric_distribution(N, K, n, k):
    """
    Calculate the probability of k successes in n draws from a finite population of size N containing K successes,
    without replacement (hypergeometric distribution).

    Parameters:
    N (int): The population size.
    K (int): The number of success states in the population.
    n (int): The number of draws.
    k (int): The number of observed successes.

    Returns:
    float: The probability of observing k successes.
    """
    return (math.comb(K, k) * math.comb(N - K, n - k)) / math.comb(N, n)


def normal_approximation_to_binomial(n, p, x1, x2):
    """
    Approximate the probability of a binomial random variable using the normal distribution.

    Parameters:
    n (int): Number of trials.
    p (float): Probability of success on each trial.
    x1, x2 (int): Range to calculate the probability for (x1 <= X <= x2).

    Returns:
    float: Approximated probability of the binomial variable within the range.
    """
    mean = n * p
    std_dev = (n * p * (1 - p)) ** 0.5
    return norm.cdf(x2, mean, std_dev) - norm.cdf(x1, mean, std_dev)


def solve_minimum_sample_size(p, z_value, E):
    """
    Solve for the minimum sample size needed using the normal approximation.

    Parameters:
    p (float): Estimated proportion (success rate).
    z_value (float): Z-value from the standard normal distribution corresponding to the desired confidence level.
    E (float): Maximum error allowed (margin of error).

    Returns:
    int: Minimum sample size required.
    """
    n = (z_value ** 2 * p * (1 - p)) / E ** 2
    return int(math.ceil(n))  # Ensure n is rounded up to the next whole number


def normal_distribution_probability(x, mean, std_dev):
    """
    Calculate the probability of a normally distributed variable being less than or equal to x.

    Parameters:
    x (float): Value to calculate the cumulative probability for.
    mean (float): Mean of the normal distribution.
    std_dev (float): Standard deviation of the normal distribution.

    Returns:
    float: Cumulative probability.
    """
    return norm.cdf(x, mean, std_dev)


def mean_and_variance_of_distribution(n, p):
    """
    Calculate the mean and variance of a binomial distribution.

    Parameters:
    n (int): Number of trials.
    p (float): Probability of success on each trial.

    Returns:
    tuple: Mean and variance of the distribution.
    """
    mean = n * p
    variance = n * p * (1 - p)
    return mean, variance


def poisson_distribution_probability(lmbda, k):
    """
    Calculate the probability of k events in a given time period for a Poisson distribution.

    Parameters:
    lmbda (float): Expected number of events in a given time period.
    k (int): Number of events to calculate the probability for.

    Returns:
    float: Probability of exactly k events.
    """
    return poisson.pmf(k, lmbda)


def find_normal_quantile(p, mean, std_dev):
    """
    Find the quantile for a given cumulative probability in a normal distribution.

    Parameters:
    p (float): Cumulative probability.
    mean (float): Mean of the normal distribution.
    std_dev (float): Standard deviation of the normal distribution.

    Returns:
    float: Quantile value.
    """
    return norm.ppf(p, mean, std_dev)


def custom_pdf_cdf(x_range, pdf_function, cdf_function=None):
    """
    Calculate the PDF and CDF for a given range and custom PDF function.

    Parameters:
    x_range (tuple): The range of x values as (min, max).
    pdf_function (function): The PDF function.
    cdf_function (function, optional): The CDF function. If not provided, will be calculated from the PDF.

    Returns:
    (np.array, np.array): Tuple of arrays representing the PDF and CDF over the given range.
    """
    x_values = np.linspace(*x_range, 1000)
    pdf_values = np.array([pdf_function(x) for x in x_values])
    if cdf_function is None:
        cdf_values = np.cumsum(pdf_values) * (x_range[1] - x_range[0]) / len(x_values)
    else:
        cdf_values = np.array([cdf_function(x) for x in x_values])
    return pdf_values, cdf_values


def bayes_theorem(prior, likelihood, marginal):
    """
    Apply Bayes' theorem to calculate the posterior probability.

    Parameters:
    prior (float): Prior probability.
    likelihood (float): Likelihood of the evidence given the hypothesis.
    marginal (float): Marginal likelihood of the evidence.

    Returns:
    float: Posterior probability.
    """
    return (likelihood * prior) / marginal


def expectation_variance_discrete(random_variable, probabilities):
    """
    Calculate the expectation and variance for a discrete random variable.

    Parameters:
    random_variable (list): The possible outcomes of the random variable.
    probabilities (list): The probabilities associated with the outcomes.

    Returns:
    (float, float): Tuple containing the expectation and variance.
    """
    expectation = sum([x * p for x, p in zip(random_variable, probabilities)])
    variance = sum([(x - expectation) ** 2 * p for x, p in zip(random_variable, probabilities)])
    return expectation, variance


def binomial_expectation_variance(n, p):
    """
    Calculate the expectation and variance for a binomial distribution.

    Parameters:
    n (int): Number of trials.
    p (float): Probability of success on each trial.

    Returns:
    (float, float): Tuple containing the expectation and variance.
    """
    expectation = n * p
    variance = n * p * (1 - p)
    return expectation, variance


def coin_toss_probability(tosses, outcomes):
    """
    Calculate the probability of a sequence of coin tosses.

    Parameters:
    tosses (int): Number of coin tosses.
    outcomes (str): Desired outcome sequence (e.g., 'HHT').

    Returns:
    float: Probability of the outcome sequence.
    """
    # Assuming a fair coin with P(H) = P(T) = 0.5
    probability = 0.5 ** tosses
    return probability


def calculate_event_probability(success_cases, total_cases):
    """
    Calculate the probability of an event.

    Parameters:
    success_cases (int): Number of successful cases.
    total_cases (int): Total number of cases.

    Returns:
    float: The probability of the event.
    """
    return success_cases / total_cases


def calculate_expectation(values, probabilities):
    """
    Calculate the expectation (mean) of a discrete random variable.

    Parameters:
    values (list): A list of values of the random variable.
    probabilities (list): A list of probabilities associated with each value.

    Returns:
    float: The expectation of the random variable.
    """
    return sum(v * p for v, p in zip(values, probabilities))


def calculate_variance(values, probabilities, expectation):
    """
    Calculate the variance of a discrete random variable.

    Parameters:
    values (list): A list of values of the random variable.
    probabilities (list): A list of probabilities associated with each value.
    expectation (float): The expectation (mean) of the random variable.

    Returns:
    float: The variance of the random variable.
    """
    return sum(p * ((v - expectation) ** 2) for v, p in zip(values, probabilities))


def chebyshevs_inequality(k, std_dev):
    """
    Calculate the bound on the probability that a value is more than k standard deviations from the mean using Chebyshev's Inequality.

    Parameters:
    k (float): The number of standard deviations from the mean.
    std_dev (float): The standard deviation of the distribution.

    Returns:
    float: The upper bound on the probability.
    """
    if k <= 1:
        return 1.0
    return 1 / k ** 2


def covariance(X, Y):
    """
    Calculate the covariance between two random variables.

    Parameters:
    X (list): A list of values for the first random variable.
    Y (list): A list of values for the second random variable.

    Returns:
    float: The covariance between X and Y.
    """
    if len(X) != len(Y):
        raise ValueError("X and Y must have the same number of elements")
    mean_X = sum(X) / len(X)
    mean_Y = sum(Y) / len(Y)
    return sum((x - mean_X) * (y - mean_Y) for x, y in zip(X, Y)) / (len(X) - 1)


def conditional_probability(joint_prob, marginal_prob):
    """
    Compute the conditional probability of A given B.

    Parameters:
    joint_prob (float): P(A and B), the joint probability of events A and B.
    marginal_prob (float): P(B), the marginal probability of event B.

    Returns:
    float: The conditional probability P(A|B).
    """
    return joint_prob / marginal_prob


def geometric_distribution_probability(p, n):
    """
    Calculate the probability of the first success on the nth trial in a geometric distribution.

    Parameters:
    p (float): The probability of success on an individual trial.
    n (int): The trial number of the first success.

    Returns:
    float: The probability of the first success on the nth trial.
    """
    return (1 - p) ** (n - 1) * p

# Example usage:
# print(chebyshevs_inequality(2, 5))
# print(covariance([10, 20, 30], [7, 14, 21]))
# print(conditional_probability(0.05, 0.1))
# print(geometric_distribution_probability(0.2, 5))
```
