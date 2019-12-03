Chapter 3: Basic Statistics: A Review
================
Mimi Wang
12/2/2019

### Problem 12

The limits of a 95% confidence interval for the mean
![\\mu](https://latex.codecogs.com/png.latex?%5Cmu "\\mu") of a normal
population with unknown variance are found by adding to and subtracting
from the sample mean a certain multiple of the estimated standard error
of the sample mean. If the sample size on which this confidence interval
is based is 28, the *multiple* referred to in the previous sentence is
the number \_\_\_\_\_\_\_\_.

``` r
multiple <- qt(0.975, df = 28 - 1, lower.tail = TRUE)
multiple
```

    ## [1] 2.051831
