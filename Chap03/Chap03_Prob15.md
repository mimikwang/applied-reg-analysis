Chapter 3: Basic Statistics: A Review
================
Mimi Wang
12/2/2019

### Problem 15

For the data of Problem 14, suppose that a test of ![H\_0:\\mu\_1 =
\\mu\_2](https://latex.codecogs.com/png.latex?H_0%3A%5Cmu_1%20%3D%20%5Cmu_2
"H_0:\\mu_1 = \\mu_2") versus ![H\_A:\\mu\_1 \>
\\mu\_2](https://latex.codecogs.com/png.latex?H_A%3A%5Cmu_1%20%3E%20%5Cmu_2
"H_A:\\mu_1 \> \\mu_2") yielded a computed value of the appropriate test
statistic equal to 2.55.

**a.** What conclusions should be drawn for ![\\alpha =
.05](https://latex.codecogs.com/png.latex?%5Calpha%20%3D%20.05
"\\alpha = .05")?

``` r
t <- qt(0.95, df = 33, lower.tail = TRUE)
t
```

    ## [1] 1.69236

Since 2.55 \> 1.69, we reject the null hypothesis.

**b.** What conclusions should be drawn for ![\\alpha =
.01](https://latex.codecogs.com/png.latex?%5Calpha%20%3D%20.01
"\\alpha = .01")?

``` r
t <- qt(0.99, df = 33, lower.tail = TRUE)
t
```

    ## [1] 2.444794

Since 2.55 \> 2.44, we reject the null hypothesis.
