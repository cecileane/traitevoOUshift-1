2016-10-06
I found a bug in package `l1ou` version 1.28.
Based on `l1ou` package version 1.28, there is still a potential problem in the package. 
We can see for covariance matrix generated by both models, their values do not match with `D{D^T}` and `B{B^T}`. So, there may be bug inside `sqrt_OU_covariance` for generating `D` and `B`. Furthermore, `B={{D^{-1}}^T}` has not been satisfied. 

Please look at the report for details:
https://github.com/yuqing19118/traitevoOUshift/blob/master/inverse_covmatrix/testingVariance.Rmd

