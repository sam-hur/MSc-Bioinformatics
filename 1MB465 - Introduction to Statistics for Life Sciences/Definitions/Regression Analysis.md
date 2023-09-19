---
tags:
  - Evergreen/Seedling
  - definition
  - statistics
  - biostatistics
---

### Definition
___
- When one variable affects the other, but not vice versa:
	e.g.:
	-  Drug conc. → heart beat
	-  Activity → condition
	- Temperature → transcription
	-  Gene duplication → genome size
- plotted with the independent variable on x (e.g. activity) and the dependent variable on the y-axis (e.g. bpm).
-  Historically one of the most applied statistical methods.
- Estimates a slope on the relationship between two variables.
- The slope is fitted to the data points using the least-squares
method, which minimizes the mean vertical distance (with
reference to y) of each observation to the fitted line
- Effect of x on y is evaluated by testing if the regression slope, b,
is significantly different from 0. ([[Null hypothesis]] H<sub>0</sub>: 𝛃 = 0)

##### Assumptions
___
- x is measured without error(!) `*`
- Linear relationship between x and y
- Residuals from the fit y ~ x are normally distributed
-  Residuals show homogeneous variance.

`*` x is assumed to be measured with more precision, as it cannot be guaranteed that it is measured without error.

#### Formulae:
___
*The Regression slope:*
$$𝑦 = 𝑏𝑥 + 𝑎$$
> Where $b$ is the slope, or <u>regression coefficient</u>.

> $a$ is the intercept, the value of $y$ as $x=0$


• The slope of a line when x predicts y **perfectly** ($r_{xy}$= 1 or -1):
$$b = [y_2 - y_1] / [x_2 - x_1] = Δy / Δx$$
	This does not work when the prediction is less than perfect (in other words, never). Then we need to calculate an averaged slope. Here, we apply the least-squares method.
	$$
	SS_E = \sum{(\hat{y}-y_i)^2}
	$$


![[Pasted image 20230915104943.png | center-align]]

___


![[Covariance#Covariance Matrices]]


![[F-Statistic#(F-statistic) Formula Regression Analysis]]


📕 For more info: *see [[F-Statistic]]



### Coefficient of Determination : $R^2$
___
- The proportion of variance in y explained by x  
- Ranges between 0 och 1.  
- If $R^2$= 0.87, then 13% of the variation in y is due to things we did not measure  
- The greater the $R^2$ the stronger the relationship  
- For simple regression: $r^2$ = $R^2$ 

![[Pasted image 20230915110757.png | center-align]]


## Polynomial Regression
___
Polynomial regression is a form of linear regression where we add some polynomial terms to linear regression to convert it into Polynomial regression due to the non-linear relationship between dependent and independent variables. 

It is a form of regression analysis in which the relationship between the independent variable x and the dependent variable y is modelled as an $n^{th}$ degree polynomial

## Multiple Regression
___
When there is more than one explanatory variable  
- Each such variable contributes to variation in y  
- The effect of one such variable (X1) on y may depend on the value of a second (X2), or third (X3)  
such variable (and so on)  
- This is an interaction between explanatory variables  
- The multiple linear regression equation is:  

$y = 𝛃_0 + 𝛃_1X_1 + 𝛃_2X_2 + ... + 𝛃_{1:2}X_1X_2$

















