### Probability
|   |   |
|---|---|
| Mutually Exclusive      | $P(A \cap B) = 0$  |
| Mutually Independent    | $P(A \cap B) = P(A)P(B)$ |
| Union                   | $P(A\cup B) = P(A)+P(B)−P(A \cap B)$ |
| Conditional Probability | $P(A \mid B) = P(A \cap B) / P(B)$ |


Bayes Theorem:
$P(A \mid B) = \frac{P(B \mid A)P(A)}{P(B)}$
Useful for Naive Bayes Classifier. Eg. P(spam|word)

### Random Variables

The value of a random variable corresponds to the occurence of some event. 


Discrete Distributions: ex. bernoulli, binomial
Continuous Distributions: ex. uniform, normal, exponential, chi-square, gamma
Note that probability of random variable taking a single value is 0.

- Probability Density Function $f(x)$:
  - Area under the curve gives probability of random variable lying in a given interval.

  - pdf takes non-negative values, with total area = 1
  

- Cumulative Density Function: $F(x)$
  Probability of random variable taking value less than x.
  - $F(x)$  = $\int_{-\infty}^{x} f(t) dt$

- Expected Value: $E[x]$
  Weighted average of all values of random variable.
  - $E[x]$  = $\int_{-\infty}^{\infty} t f(t) dt$

### Statistics
- Mean: average value
$\mu = E[x]$ 
- Variance: spread of values
$\sigma = E[(X-E[X])^2] = E[X^2] - (E[X])^2 $
- Bias: average deviation of estimator/prediction from actual value

- Covariance: 
$\sigma_{XY} = E[(X-E[X])(Y-E[Y])]$
$\sigma_{XY} = E[XY]-E[X]E[Y]$

- Correlation: 
$\rho_{XY} = \sigma_{XY}/\sigma_X\sigma_Y$
value of -1 or 1 signifies complete dependence
value of 0 signifies independence

For ML,
- Overfitting: low bias in training, high variance
(Adjusts very well to training data but accuracy drops with new test data)
- Underfitting: high bias in training, low variance

- Accuracy:  (TP+TN) / Total 
--> fraction of correct predictions
- Precision: TP / (TP+FP) 
--> fraction of predicted positives that were true
- Recall: TP / (TP+FN)
--> fraction of actual positives that were identified correctly

Note: a model may only predict 10% of positives correctly, but its precision maybe high if false positives are also low. Therefore recall is also important.

- F1 score: harmonic mean of precision and recall.

