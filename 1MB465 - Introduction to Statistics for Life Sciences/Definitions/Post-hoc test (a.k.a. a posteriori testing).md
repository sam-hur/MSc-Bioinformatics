---
tags:
  - Evergreen/Seedling
  - definition
  - statistics
  - biostatistics
---
### Definition
---
In a scientific study, post hoc analysis consists of statistical analyses that were specified after the data were seen. They are usually used to uncover specific differences between three or more group means when an analysis of variance test is significant.



### Tests:
---
##### **Tukey's HSD**
Tukey's Honest Significant Difference (HSD) test is a post hoc test commonly used to <u>assess the significance of differences between pairs of group means</u>. Tukey HSD is often a follow-up to one-way ANOVA, when the F-test has revealed the existence of a significant difference between some tested groups.

###### Assumptions
The assumptions are:
- The observations are **independent**,
- **normality** of distribution,
- **homogeneity of variance**.

---
NB: these are the same assumptions as for [[One-Way ANOVA]]; in other words, if you were allowed (or if you allowed yourself) to conduct an [[Analysis of Variance (ANOVA)]] test, then it is OK to run Tukey’s test.
___

###### Formulae
- Critical q value
$$
q = \frac{\bar{X}_A - \bar{X}_B}{SEM}
$$

(See note on [[Standard Error (of the Mean) - SEM]])
![[Standard Error (of the Mean) - SEM#Formulae]]




##### **Bonferroni test**
The Bonferroni test is a type of multiple comparison test used in statistical analysis. When performing [[hypothesis testing]] with multiple comparisons, eventually a result could occur that appears to demonstrate [statistical significance](https://www.investopedia.com/terms/s/statistical-significance.asp) in the dependent variable, even when there is none.

If a particular test, such as a linear regression (or alternatively an [[Analysis of Variance (ANOVA)]]), yields correct results 99% of the time, running the same regression on 100 different samples could lead to at least one false-positive result at some point. The Bonferroni test attempts to prevent data from incorrectly appearing to be statistically significant like this by making an adjustment during comparison testing.

