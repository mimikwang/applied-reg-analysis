Chapter 3: Basic Statistics: A Review
================
Mimi Wang
12/1/2019

### Problem 4

**a.** ![P(\\chi\_7^2 \\geq ?)
= 0.01](https://latex.codecogs.com/png.latex?P%28%5Cchi_7%5E2%20%5Cgeq%20%3F%29%20%3D%200.01
"P(\\chi_7^2 \\geq ?) = 0.01")

``` r
# Get the limit
lim <- qchisq(0.01, df = 7, lower.tail = FALSE)

# Visualize
x1 <- seq(-1, 25, length = 200)
y1 <- dchisq(x1, df = 7)
plot(x1, y1, lwd = 2, type = "l",
  xlab = "x", ylab = "y", main = TeX(paste("$P(\\chi_7^2 \\geq", round(lim, 2),") = 0.01")))

x2 <- seq(lim, 25, length = 200)
y2 <- dchisq(x2, df = 7)
polygon(c(lim, x2, 25), c(0, y2, 0), col = "gray")
```

![](Chap03_Prob04_files/figure-gfm/unnamed-chunk-1-1.png)<!-- -->

**b.** ![P(\\chi\_12^2 \\leq 14) =
?](https://latex.codecogs.com/png.latex?P%28%5Cchi_12%5E2%20%5Cleq%2014%29%20%3D%20%3F
"P(\\chi_12^2 \\leq 14) = ?")

``` r
# Get the Probability
prob <- pchisq(14, df = 12, lower.tail = TRUE)

# Visualize
x1 <- seq(-1, 40, length = 200)
y1 <- dchisq(x1, df = 12)
plot(x1, y1, lwd = 2, type = "l",
  xlab = "x", ylab = "y", main = TeX(paste("$P(\\chi_7^2 \\leq 14) =", round(prob, 2))))

x2 <- seq(-1, 14, length = 200)
y2 <- dchisq(x2, df = 12)
polygon(c(-1, x2, 14), c(0, y2, 0), col = "gray")
```

![](Chap03_Prob04_files/figure-gfm/unnamed-chunk-2-1.png)<!-- -->
