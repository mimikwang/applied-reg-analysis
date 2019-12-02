Chapter 3: Basic Statistics: A Review
================
Mimi Wang
12/1/2019

### Problem 9

Find the **(a)** mean, **(b)** median, and **(c)** variance for the
following set of scores:

{0, 2, 5, 6, 3, 3, 3, 1, 4, 3}

``` r
scores <- c(0, 2, 5, 6, 3, 3, 3, 1, 4, 3)

# mean
mean(scores)
```

    ## [1] 3

``` r
# median
median(scores)
```

    ## [1] 3

``` r
# variance
var(scores)
```

    ## [1] 3.111111

**d.** Find the set of Z scores for the data.

``` r
z_scores <- (scores - mean(scores)) / (var(scores))
z_scores
```

    ##  [1] -0.9642857 -0.3214286  0.6428571  0.9642857  0.0000000  0.0000000
    ##  [7]  0.0000000 -0.6428571  0.3214286  0.0000000
