Chapter 3: Basic Statistics: A Review
================
Mimi Wang
12/2/2019

### Problem 11

Suppose that the weight ![W](https://latex.codecogs.com/png.latex?W "W")
of male patients registered at a diet clinic has the normal distribution
with mean 190 and variance 100.

**a.** For a random sample of patient of size ![n
= 25](https://latex.codecogs.com/png.latex?n%20%3D%2025 "n = 25"), the
expression ![P(\\overline{W}
\< 180)](https://latex.codecogs.com/png.latex?P%28%5Coverline%7BW%7D%20%3C%20180%29
"P(\\overline{W} \< 180)") in which
![\\overline{W}](https://latex.codecogs.com/png.latex?%5Coverline%7BW%7D
"\\overline{W}") denotes the sample mean weight, is equivalent to saying
![P(Z \> ?)](https://latex.codecogs.com/png.latex?P%28Z%20%3E%20%3F%29
"P(Z \> ?)"). \[*Note:* ![Z](https://latex.codecogs.com/png.latex?Z "Z")
is a standard normal random variable.\]

``` r
z_score <- (190 - 180) / (sqrt(100) / sqrt(25))
z_score
```

    ## [1] 5

**b.** Find an interval ![(a,
b)](https://latex.codecogs.com/png.latex?%28a%2C%20b%29 "(a, b)") such
that ![P(a \< \\overline{W} \< b) =
.80](https://latex.codecogs.com/png.latex?P%28a%20%3C%20%5Coverline%7BW%7D%20%3C%20b%29%20%3D%20.80
"P(a \< \\overline{W} \< b) = .80") for the same random sample in part
(a).

``` r
a <- qnorm(0.90, mean = 190, sd = sqrt(100) / sqrt(25), lower.tail = FALSE)
b <- qnorm(0.90, mean = 190, sd = sqrt(100) / sqrt(25), lower.tail = TRUE)

a; b
```

    ## [1] 187.4369

    ## [1] 192.5631
