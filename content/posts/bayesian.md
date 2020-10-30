+++
title = "Learning Python, R, and Julia with Bayesian statistics Stats Setupfile"
author = ["Justin Ochalek"]
draft = false
+++

## Why do this? {#why-do-this}

It has been more than 10 years since I learned statistics. In order to brush up on the subject I have been working through Will Kurt's aptly named **Bayesian Statistics the Fun Way**. I want to learn a bit of Python, R, and Julia while I'm at it.

Let's pretend I receive 12 interview invitations for medical school, but I get a lot of anxiety about being interviewed. I am so anxious about it that I only want to attend enough interviews to have a good chance of getting two offers. I've got a lot of social anxiety, so a 20% chance of getting two admission offers is good enough for me. Based off of my MCAT score, I have a 10% chance of getting accepted after an interview. It looks like if I attent nine interviews, I will have a 22.5% of getting into two schools.

The book makes learning statistics easy, but don't take my word for it...

‘<https://nostarch.com/learnbayes/>’


## Python {#python}

In

```python
from scipy.stats import binom
print(1-binom.cdf(1, 9, (1/10)))

```

```text
0.22515902199999993
```

Out

```text
0.22515902199999993
```


## R {#r}

In

```R
pbinom(1,9,1/10,lower.tail = FALSE)

```

```text
[1] 0.225159
```

Out

```text
[1] 0.225159
```


## Julia {#julia}

In

```julia
using Distributions
1-cdf(Binomial(9, 1/10), 1)

```

```text

0.22515902200000015
```

Out

```text

0.22515902200000015
```
