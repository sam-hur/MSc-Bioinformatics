---
tags:
  - Evergreen/Seedling
  - definition
  - statistics
  - biostatistics
---


## Definition
___
- A value obtained from running an [[Analysis of Variance (ANOVA)]] test or [[Regression Analysis 2]], which is used to find out whether the means are significantly different.
- Similar to a t statistic from a [[Students t-test]]. However, where a [[Students t-test]] will tell you if a <u>single</u> variable is statistically significant, an F-test will tell you if a <u>group</u> of variables is jointly significant.


#### Use:
___
- When deciding to support or reject the [[Null hypothesis]] or [[Alternative hypothesis]]

###### F-Value and F-Critical Value
- The F value is a value that is calculated from the data and is also called the **F-statistic**
- The F-Critical Value is a specific value to which the F-Value is compared. Generally, *if your calculated F value in a test is larger than your F critical value, you can reject the null hypothesis*.

- Once an F-statistic is calculated, its significance can be asses by looking up the critical value under the null hypothesis in the [[F-distribution table]] (See Below).

##### Key info
___
- The F statistic <u>must be</u> used in combination with the [[P-value]].



#### F-Statistic: formula
___

###### (F-statistic) Formula: [[Analysis of Variance (ANOVA)]]
$$F = \frac{MS_b}{MS_w}$$
###### (F-statistic) Formula: [[Regression Analysis 2]]
$$
\sum{y_i - \bar{y}} = \sum{(\hat{y} - \bar{y})^2 + \sum{(y_i - \hat{y})}}
$$

$$
SS_R = SS_T -SS_E = \sum^i_{i=1}{(\hat{y_i} - \bar{y})^2}
$$
![[Pasted image 20230915105949.png|center-align]]


#### (snippet) [[Analysis of Variance (ANOVA)]]
___
![[Analysis of Variance (ANOVA)#Variance of means]]

![[Analysis of Variance (ANOVA)#Mean Squares]]
📕 For more info: *see [[Analysis of Variance (ANOVA)]]


### Video help
___

![Intro to the F-Statistic](https://www.youtube.com/watch?v=Uh2ky5RXkeA&ab_channel=TheOrganicChemistryTutor)

___
### Distribution table

![[F-distribution table]]


