+++
title = "Using Python Math with Bayesian statistics just for fun"
author = ["Justin Ochalek"]
draft = false
+++

## Initialize the python session to be used in SRC blocks {#initialize-the-python-session-to-be-used-in-src-blocks}

Use the same ":session" in each python source block to maintain the same environment

```emacs-lisp
(org-babel-do-load-languages
  'org-babel-load-languages
   '((python t)))
(pyvenv-activate "~/path/to/environment/.venv")
```


## Python blocks {#python-blocks}

```python
from scipy.stats import binom
x = [1]
print(1-binom.cdf(1, 7, (1/5)))


```

```text
0.42328319999999986
```


## 1 {#1}

k = 1, n = 12, p = 1/10


## 2 {#2}

16 ways


## 3 {#3}

0.0004548552879040868


## 4 {#4}

0.2752512000000002


## 5 {#5}

0.1877066233635499
More likely to get a job with just 7 interviews while not tired.

```python
import statistics as stats
A = [2, 4, 6]
B = stats.mean(A)
print(B)

```


## R blocks {#r-blocks}

```R
pbinom(1,7,1/5,lower.tail = FALSE)

```


## Julia blocks {#julia-blocks}

```julia


```
