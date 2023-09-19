---
tags:
  - Evergreen/Seedling
  - definition
  - statistics
  - biostatistics
Type: []
---

## Definition
___
*Analysis of Variance (ANOVA)* is a collection of statistical models and their associated estimation procedures used to analyze the differences among means. ANOVA was developed by the statistician [Ronald Fisher](https://en.wikipedia.org/wiki/Ronald_Fisher).

It is a statistical technique used to analyze the differences among the means of two or more groups or treatments. It is primarily used to determine whether there are statistically significant differences between group means. ANOVA does this by comparing the variability between the groups (due to differences in group means) to the variability within the groups (due to random variation or error). <u>If the between-group variability is significantly greater than the within-group variability, ANOVA suggests that there are differences among the groups being studied.</u>


“*This test generates a statistic, which increases in size as the difference between two or more means increases*”

#### Underlying Thinking and Logic
___
The logic behind ANOVA is rooted in comparing variances. It seeks to answer whether the variability between groups is greater than the variability within groups. Here are some key aspects of the underlying thinking:

1. **Variability Comparison**: ANOVA is designed to partition the total variability observed in the data into two components: the variation due to differences between groups and the variation due to random error within groups.

2. [[Hypothesis Testing]]: ANOVA formulates null and alternative hypotheses. The null hypothesis assumes that there are no significant differences among the group means, while <u>the alternative hypothesis suggests that at least one group mean is different from the others</u>.

3. [[F-statistic]]: ANOVA computes an F-statistic by comparing the ratio of between-group variability to within-group variability. If the F-statistic is sufficiently large, it indicates that at least one group mean differs significantly from the others.

4. [[Post-hoc test (a.k.a. a posteriori testing)]]: If ANOVA suggests significant differences among groups, post-hoc tests can be performed to identify which specific groups differ from each other.

5. **Assumptions**: ANOVA assumes that the data are normally distributed within each group, the variances are approximately equal between groups (homoscedasticity), and that observations are independent.
	1. Note: Many authors suggest preliminary testing for homoscedasticity is **not** necessary, provided that, <u>as a very general rule</u>, the ratio of the largest to smallest variance does not exceed 4:1.
 
### Thinking Process
___
1. First, consider the case where <u>none of the factors</u> have any effect on the response variable.
	1. Ask: “Why is there variation <u>among the individuals within each group</u>? Why isn't the value for each individual the same as its group mean?”.
		1.  Because of individual variation that we cannot do anything about.
	- ↑ *This inherent and uncontrollable variable  is often called '**error**'* 
	2. Ask: “Why is there variation <u>among the group means</u>? Why isn't each factor the same as the grand mean?“
		1. Because of individual variation that we cannot do anything about.
	3. You can quantify the amount of variation around a mean by calculating the variance (Ch. 8, Steve McKillup – Statistics Explained: An introductory guide for life scientists).
		1. Two separate variances:
			1. Individual variance around their respective group means.
			2. Group variance around the grand mean.
2. Second, consider the case where some/all factors <u>do</u> have an effect on the response variable.
	1. Repeat the above (Step 1.1)!
	2. Repeat Step 1.2
		1. (Step 1.2.1) it is <u>not just caused by error – it is also caused by the effects of the factor</u>.
		2. Therefore, the variance of the group means around the grand mean will be much larger than if the variance in group means was caused only by *error* as it is caused by the **factor + error**
			1. This gives a very easy way to calculate a statistic that shows <u>how much difference there is among treatment means, over and above that expected because of natural/individual variation</u> (i.e., *error*). 

___

##### Variance of means
- The variance of the group means (e.g., treatment groups) around the grand mean indicated **treatment + error** and is called the *among group variance*.
$$MS_b$$

- The variance of the individuals around their respective group means indicated **only error** and is called the *within group variance*
$$
MS_w
$$
##### F-Statistic

![[F-Statistic#(F-statistic) Formula Analysis of Variance (ANOVA)]]


📕 For more info: *see [[F-Statistic]]*
___


#### Common types of ANOVA include:
___
- [[One-Way ANOVA]]: Compares means across two or more independent groups.

- [[Two-Way ANOVA]]: Examines the effects of two independent variables (factors) on a dependent **response variable**. It can assess both main effects and interaction effects.

- [[Repeated Measures ANOVA]]: Used when measurements are taken on the same subjects at multiple time points or under different conditions.

##### One Way vs. Two-Way ANOVA (Diagram)
___

![[statwork2.jpg | center-align]]

> Note: an independent variable is a *factor* 


## Formulae
___
### Sum of Squares
#### Total Variance
$$
SS_T = \sum_{i=1}^{k}\sum_{j=1}^{n_i}(X_{ij} - \bar{X})^2
$$
Where:

- $k$ is the number of groups or treatments.
- $n_i$​ is the sample size of group $i$.
- $X_{ij}$​ is the $j$<sup>th</sup> observation in group $i$.
- $\bar{X}_i$​ is the mean of group $i$.



### Mean Squares:
##### Mean Square Between
$$MS_b = \frac{SS_b}{df_b}$$
Where $b$ = between, and $df$ = degrees of freedom



##### Mean Square Within
$$
MS_w = \frac{SS_w}{df_w}
$$
Where $w$ = within, and $df$ = degrees of freedom

### Calculating the F-Statistic:
![[F-Statistic#F-Statistic formula]]
📕 For more info: *see [[F-Statistic]]*

#### P-value
The p-value is used to determine the statistical significance of the F-statistic. It depends on the F-distribution with $df_b$​ and $df_w$ degrees of freedom.

##### Critical Value
You can compare the calculated F-statistic to the critical value from the [[F-distribution table]] to determine significance.

### Factors
___
> **A fixed factor is** one where the treatments (e.g., levels of temperature) have been **specifically chosen**

> A random factor is one where the treatments are used as random representatives of the full set of possible treatments within that factor.
> 
> 	Therefore, the [[null hypothesis]] is more general. (e.g., “here is no difference in cockroach activity at different temperatures. The levels of temperature chosen and used in the experiment in this case are **random representatives** of the wider range of temperatures that the cockroaches may experience”).



