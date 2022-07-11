# Learnable inductive biases in Neural Netrok

- Mark van der Wilk

---

- Growing research group focusing on
  - Gaussian process inference 
    - backgred by theory to make
    - reliable decision making systems
  - automatic learning of inductive vias in neural works
    - When should neurons be connected?

---

- Hyperparameter selction and architecture design

---

- Every time we train a NN we need to decide on hyperparameters
  - How many layers?
  - hOW MANY UNITS IN A layer?
  - What layer structure?
  - Convolutional? Skip connections?
  - Data argumentation parameters?
- As architectures get more complex
  - Multi task
  - Which layers to share?
  - What kind of task specific layers?
  - How much capacilty to assign to each task

---

- Main tool is trail and error
- cross validation

## Invariances

- Every prediction problem needs an inductive bias
- f
- x, image
- y, label
- inductive bias
  - for the unseen bias

---

- Architecture determins inductive vias through equivariances
  - Convolutions are a common solution
  - translational variances

----

- Can we automatically adjust invariance properties in layers?

---

## Summary

- Goal
  - Given a dataset
  - adapt the inductive bias to it
- key requirements
  - find a parameterisation for different inductive biases
  - Find a learning objective that works for inductive viases 
    - We want to optimise it through backprop
      - So it is easy
- We will look at
  - Invariances and equivariances parameterised though
    - Transformations on the input
      - data argumentation
    - transformations on the filter
      - convolutions
  - how bayes helps with finding a learning objective
  - Single layer and deep models

## Invariance, data argumentation and training loss

## Data argumentation

- Take a dataset

- 
  $$
  y=\{(x_n, y_n)\}_{n=1}^N
  $$
  

- Create larger dataset

- $$
  y'=\{\}
  $$

  

## Making models invariant

- $$
  f(x)=f(t_i (x))
  $$

  

$$
w^*
$$

$$
f(x)=f(t_i(x))
$$

$$
p(t|\theta)
$$

$$
\theta 
$$

- amount of different transformations to apply

- what if we do not know the transformations for which 

- $$
  f(x)=f(t_i(x))
  $$

  

$$
\theta
$$

$$
w^*,\theta^*=\mathop{min}\limits_{w,p}
$$

$$
p(t|\theta)
$$

## Bayesian model selection

$$
f_{w,\theta}=\phi_\theta(x)^T W = \sum_{i=1}^K \phi_\theta^{(i)}(x)w_i
$$

$$
L_{train}
$$

$$
p(f,\theta|y)=\frac{p(y|f)p(f|\theta)p(\theta)}{p(y)}=\frac{p(y|f)p(f|\theta)}{p(y|\theta)}\frac{p(y|\theta) p(\theta)}{p(y)}
$$

$$
p(y|\theta)=\int
$$

$$
NN
$$

$$
ELBO
$$

## Learning data augumentation

- Formulate data learning data argumentations as Bayesian hyperparameter learning

$$
f_{w,\theta}(x)=\mathbb{E}_{p(t|\theta)[\phi_\theta (t(x))^T w]}
$$

$$
p(y_n|w,\theta)=\mathcal{N}
$$

$$
log p (y | \theta) \ge \mathcal{L}=\sum_{n} \mathbb{E}_{q(w)}[log p (y_n|\mathbb{E}_{p(t|\theta)})]
$$

$$
log p (y|\theta) \ge
$$

$$
\mathcal{L}(q(w),\theta)
$$

$$
p(t|\theta)
$$

$$

$$

- one model
- two in two problems

$$
\mathcal{L}(q(\bold{w}),\theta)
$$

$$

$$

## Learning equivariance

- previously
- added invariance by transforming the input image

$$
f_{\bold{w}, \theta} (\bold{x})=\mathbb{E}_{p(t|\theta)}[\phi]
$$

$$

$$

## Single architecture for different domains

- Learning invariances using the Marginal Likelihood
  - Learning invariance by backprop 
  - But Gaussian processes only
- Data argumentation in BNNs and the cold posterior effect
  - Whether a principled approach to DA influences the gold
- 

## Summary

- Given a dataset
- adapt the inductive bias to it

## Key requirements

- parameterisation
- learning objective
  - Backprop
- invariances

## Outlook

- better than trial and error design NNs
- Bayesian methods are helping the automation of selecting invariances
  - making ity as easy as backprop
- Can nake NNs 
  - More accurate 
  - easier to use
  - more energy efficient 
- Get to the smarter neuron!
  - Meta learning
  - More Bayes?
  - Causality?
  - 