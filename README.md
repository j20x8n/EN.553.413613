java c



Applied Stats and Data AnalysisEN.553.413-613, Spring 2024Feb 21, 2024Exam 1







Question 1 (18 pts). The following TRUE/FALSE questions concern the Simple LinearRegression modelYi = β0 + β1Xi + εi, E(εi) = 0, V ar(εi) = σ2, cov(εi, εj ) = 0, for i = j.(a) TRUE or FALSE. For the least squares estimates b0, b1 we require the errors to benormally distributed.(b) TRUE or FALSE. The estimated mean of the response variable at Xiis defined asb0 + b1Xi.(c) TRUE or FALSE. One of the Gauss Markov conditions is P ni=1 ei = 0.(d) TRUE or FALSE. Plotting e2i vs Yˆiis one of the diagnostic plots.(e) TRUE or FALSE. QQ plot of the Yi’s is one of the diagnostic plots.(f) TRUE or FALSE. Low R2 means that X and Y are not related.(g) TRUE or FALSE. The s2is an estimate of the variance of Yi.(h) TRUE or FALSE. Coefficient of simple determination R2 measures the proportion of theexplained variation in Y over the unexplained variation in Y .(i) TRUE or FALSE. In the Correlation model of the regression Xi’s are random variables.









Question 2 (18 pts). Let X, Y, Z ∼ iid N(0, 1), i.e. they are independent, identicallydistributed standard normal random variables. For the following random variables statewhether they follow a normal distribution, a t- distribution, a χ2 distribution, an Fdistribution, or none of the above. State relevant parameters (e.g. degrees of freedom,and means and variances for normal RVs)







(a) 3Y − Z(b) X + Y + Z.(c) X2 + Y2 + Z2.X2 + Y2(d)2Z2X2(e) √Y2 + Z2(X + Y )2(f)2







Question 3 (20 pts). Suppose a data set {(Xi, Yi) : 1 ≤ i ≤ n} is fit to a linear model ofthe form.Yi = β0 + β1xi + εiwhere εi are independent, mean zero, and normal with common variance σ2. Here we treatY as the response variable and X as the predictor variable. The output of the lm functionis given. Some values are hidden by ‘XXXXX’. We provide you with additional value:X¯ = 1.11.Coefficients:Estimate Std. Error t value Pr(>|t|)(Intercept) 1.9412 0.4593 4.226 0.000508 ***x 0.7042 0.3697 1.905 0.072911 .---Signif. codes: 0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1Residual standard error: 0.9221 on 18 degrees of freedomMultiple R-squared: 0.1678, Adjusted R-squared: -----F-statistic: XXXXX on XX and XX DF, p-value: XXXXXX(a) (2 points) How many data points are there (what is n, the sample size)? What is theestimated mean of the response variable Y at Xh = 2 for this dataset?(b) (3 points) Based on all of this output, do you reject H0 : β1 = 0 in favour of Ha : β1 = 0at level α = 0.05 significance? What does the test tell us about the relationship betweenX and Y ?(c) (3 points) Based on all of this output, do you reject the H0 : β1 = 0 vs Ha : β1 > 0 atlevel α = 0.05 significance? Briefly explain why, or why not.(d) (4 points) The degrees of freedom, the p-value and the value of the F statistic are hidden.Is it possible to reconstruct all of them based on the data shown? Recover as many valuesas you can.(e) (4 points) Based on the data above find SSTo, SSR and SSE. Hint: Residual standarderror may be useful here.(f) (4 points) Find the 95% confidence interval for the mean of the response function atXh = 2. Write your answer in the form. A ± B · t(C, D), specify values A, B, C, D asprecise as you can (i.e. find values of as many terms as you can).





Question 4 (14 pts). Consider the following diagnostic plots for two models (Model 1 andModel 2). Two simple linear regression models Y = β代 写EN.553.413-613, Spring 2024 EN.553.413-613, Spring 2024 Exam 1SQL
代做程序编程语言0 + β1X + ε are fitted to the twodifferent datasets (X, Y ) observations of each Model. For each model 3 diagnostic plots areshown: plot of Yi vs Xi, plot of semi-studentized residuals e∗i versus fitted values Yˆi, QQ-plotof the semi-studentized residuals e∗i.









(a) (5 points) What is the main issue do you diagnose with the Model 1, if any? Why?Which plot was the most useful in diagnosing this problem? Be as specific in describingthe issue as you can.(b) (5 points) What is the main issue do you diagnose with the Model 2, if any? Why?Which plot was the most useful in diagnosing this problem? Be as specific in describingthe issue as you can.(c) (4 points) This question is unrelated to the above plots. Explain in what cases thetransformation of the predictor variable X is more appropriate than the transformationof the response variable Y .





Question 5 (20 points). For the dataset of n = 200 observations a simple linear regressionmodel Yi = β0 + β1Xi + εiis fit. The following estimates are obtained.b0 = 2, b1 = 1We have listed additional information here









(a) (2 points) What is the estimated variance s2 of the error term based on the data above?(b) (3 points) Find a 90% confidence interval for β1. Write it in the form. A ± B · t(C, D),compute values of A, B, C, D if possible.(c) (4 points) Find the joint confidence intervals with confidence at least 90% for β0, β1 inthe form. Ai ± Bi· t(Ci, Di). Compute values of Ai, Bi, Ci, Diif possible. Without anycomputation how does the interval for β1 for this part compare to the one in part (a)?(d) (4 points) Find the joint confidence intervals using Bonferroni procedure with confidenceat least 90% for the mean of the response variable at Xh = 2 and Xh′= 0. Find it inthe form. Ai ± Bi· t(Ci, Di).(e) (4 points) Set up a General Linear Test for the data provided: specify the reduced andfull model, compute the value of the F-statistic, specify its distribution under the nullhypothesis.(f) (3 points) An Aspiring Data Scientist (ADS) noticed that one of the observed data points(Xi, Yi) = (2, 15) lies outside of the 99% Working-Hotelling band (we assume everythingwas computed correctly). They claim it is an issue. Briefly justify if their concern iscorrect or not.









Question 6 (20 points). Suppose Yifollows the modelYi = βXi + εiwhere εiis independent, identically distributed N(0, σ2). Note, there is no intercept term.You observe a collection {(Xi, Yi)} of data from this model, i = 1, . . . , n.(a) (5 points) Write the objective function to be minimized and the equations that need tobe solved to get the least squares estimate of β.(b) (5 points) Solve the equation in (a) and express the answer as a linear combination ofYi’s.(c) (5 points) What is the distribution of b? Find the mean, variance. Justify your steps(d) (5 points) Write the log-likelihood that needs to be maximized to obtain the estimate ofβ. DO NOT MAXIMIZE IT.(a) Function to be minimized







Equations to be solved:





(b) Solving the equation:



(c) Since b =PiciYi, a linear combination of normal RVs, it will be a normal RV itself.The mean is









The variance is









We have shown that







(d) The log-likelihood is



















         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
