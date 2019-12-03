Chapter 3: Basic Statistics: A Review
================
Mimi Wang
12/2/2019

### Problem 13

A random sample of 32 persons attending a certain diet clinic was found
to have lost (over a three-week period) an average of 30 pounds, with a
sample standard deviation of 11. For these data, a 99% confidence
interval for the true mean weight loss by all patients attending the
clinic would have limits (?, ?).

``` r
lower <- qnorm(0.995, mean = 30, sd = 11 / sqrt(32), lower.tail = FALSE)
upper <- qnorm(0.995, mean = 30, sd = 11 / sqrt(32), lower.tail = TRUE)

lower; upper
```

    ## [1] 24.99119

    ## [1] 35.00881
