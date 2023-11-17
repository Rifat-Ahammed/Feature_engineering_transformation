# Feature_engineering_transformation

A brief description of what this project does and who it's for.

Here, I tried to explain everything about transformation.
 
This project is for beginners who are totally new in ML and Data Science.
## Normalization 

It's a really good idea to write all steps on paper and try to understand how it is working mathematically, then implement it in Code. 

```bash
    Initially decalre these 2 python libraries

    import pandas as pd
    import numpy as np
  
```

```bash
    Formula X = (X(i) - min(X)) / (max(X) - min(x))

    library: from sklearn.preprocessing import MinMaxScaler

```
## Standardization 

```bash
    Formula X = (X(i) - X(mean)) / standard deviation

    standard deviation σ = sqrt(sum(X(i) - μ)^2) / N

    Where
        σ = Population standard deviation
        N = the size of Population
        X(i) = Each value from the Population
        μ = the Population mean
        
    library: from sklearn.preprocessing import StandardScaler

```

## Log Transformation

```bash
    Formula log1p = loge(1+x)

    library: from sklearn.preprocessing import FunctionTransformer

```
## Robust Scaler 

### Note: Before going to the Mathematical term we have to sort the dataset in ascending order. 
```bash
    Formula X(scale) = (X(i) - X(med)) / (X(75) - X(25))

    Where

        X(med) = 50th quantile = 2/4(n+1)
        X(75) = 75th quantile = 3/4(n+1)


    library: from sklearn.preprocessing import RobustScaler

```

## Max Absolute Scaler


```bash
    Formula X(scale) =abs( X / max(x))

    library: from sklearn.preprocessing import MaxAbsScaler
```


## Author

- [@Rifat-Ahammed](https://github.com/Rifat-Ahammed)
