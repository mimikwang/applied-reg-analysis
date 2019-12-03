Chapter 3: Basic Statistics: A Review
================
Mimi Wang
12/2/2019

### Problem 14

From two normal populations assumed to have the same variance,
independent random samples of sizes 15 and 19 were drawn. The first
sample (with ![n\_1
= 15](https://latex.codecogs.com/png.latex?n_1%20%3D%2015 "n_1 = 15"))
yielded mean and standard deviation 111.6 and 9.5, respectively, while
the second sample (![n\_2
= 19](https://latex.codecogs.com/png.latex?n_2%20%3D%2019 "n_2 = 19"))
gave mean and standard deviation 100.9 and 11.5, respectively. The
estimated standard error of the difference in sample means is
\_\_\_\_\_\_\_.

The equation for pooled variance:   
![S\_p^2 = \\frac{(n\_1 - 1)S\_1^2 + (n\_2 - 1)S\_2^2}{n\_1 + n\_2
- 2}](https://latex.codecogs.com/png.latex?S_p%5E2%20%3D%20%5Cfrac%7B%28n_1%20-%201%29S_1%5E2%20%2B%20%28n_2%20-%201%29S_2%5E2%7D%7Bn_1%20%2B%20n_2%20-%202%7D
"S_p^2 = \\frac{(n_1 - 1)S_1^2 + (n_2 - 1)S_2^2}{n_1 + n_2 - 2}")  

The equation for standard error:   
![SE = S\_p \\sqrt{\\frac{1}{n\_1} +
\\frac{1}{n\_2}}](https://latex.codecogs.com/png.latex?SE%20%3D%20S_p%20%5Csqrt%7B%5Cfrac%7B1%7D%7Bn_1%7D%20%2B%20%5Cfrac%7B1%7D%7Bn_2%7D%7D
"SE = S_p \\sqrt{\\frac{1}{n_1} + \\frac{1}{n_2}}")  

``` r
# First, calculate the pooled sample variance
var_pooled <- ((15 - 1) * 9.5^2 + (19 - 1) * 11.5^2) / (15 + 19 - 2)

# Then calculate the standard error
se <- sqrt(var_pooled) * sqrt(1 / 15 + 1 / 19)
se
```

    ## [1] 3.685795
