# Model

## Deterministic Model

Discriminative models draw boundaries in the data space, while generative models try to model how data is placed throughout the space. A generative model focuses on explaining how the data was generated, while a discriminative model focuses on predicting the labels of the data.

In the case of discriminative models, to find the probability, they directly assume some functional form for $P(Y|X)$ and then estimate the parameters of $P(Y|X)$ with the help of the training data.

## Generative Model

In the case of generative models, to find the conditional probability $P(Y|X)$, they estimate the prior probability $P(Y)$ 
and likelihood probability $P(X|Y)$ with the help of the training data and uses the Bayes Theorem to calculate the posterior probability $P(Y |X)$.

$$
P(Y|X) = \text{posterior} = \frac{prior \times likelihood}{evidence}  = \frac{P(Y) P(X|Y)}{P(X)}
$$

### Autoregressive

An AR(1) autoregressive process is one in which the current value is based on the immediately preceding value,
while an AR(2) process is one in which the current value is based on the previous two values.
An AR(0) process is used for white noise and has no dependence between the terms.

??? cite "Autoregressive"
    By JASON FERNANDO  

    A statistical model is autoregressive if it predicts future values based on past values.
    For example, an autoregressive model might seek to predict a stock's future prices based on its past performance.

    - Autoregressive models predict future values based on past values.
    - They are widely used in technical analysis to forecast future security prices.
    - Autoregressive models implicitly assume that the future will resemble the past.
    - Therefore, they can prove inaccurate under certain market conditions, such as financial crises or periods of rapid technological change.

    [original text](https://www.investopedia.com/terms/a/autoregressive.asp)


## Get Models

### Pytorch Models

- [Pytorch Models & Pre-trained Weights](https://pytorch.org/vision/stable/models.html)

### ModelZoo

- [ModelZoo](https://modelzoo.co/)


### Pytorch Image Models (timm)

- [GitHub Repository](https://github.com/fastai/timmdocs/tree/master/)
- [official doc](https://rwightman.github.io/pytorch-image-models/)
- [fastai's doc](https://fastai.github.io/timmdocs/#)
