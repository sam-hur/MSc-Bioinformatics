---
tags:
  - Evergreen/Seedling
  - definition
  - statistics
  - biostatistics
---

## Definition
___
The standard error of a statistic is the standard deviation of its sampling distribution or an estimate of that standard deviation. If the statistic is the sample mean, it is called the standard error of the mean


**The standard error of the mean (SEM)** **measures how much discrepancy is likely in a sample's mean compared with the population mean**. The SEM takes the SD and divides it by the square root of the sample size. <u>The SEM will always be smaller than the SD</u>.

Shows you how good your data is
- It does this by providing more insight on the mean than a simple bar graph (without error bars) would (e.g., by showing how distored the data is - as can be judged by the size of the error bars).
- It takes the standard deviation and divides it by the square root of the sample size:
	

### Formulae
___

- Single sample, where $S$ is the standard deviation of the sample.
$$	SEM_\bar{x} = \frac{S}{\sqrt{n}} $$



- Equal sample sizes, where MSE is the Mean Square Error ([[Regression Analysis 2]])

$$
SEM = \sqrt{\frac{MSE}{n}}
$$

- Different sample sizes (e.g., [[Students t-test]] or [[Analysis of Variance (ANOVA)]])

$$
SEM = \sqrt{\frac{MSE}{2} × (\frac{1}{n_A}+\frac{1}{n_B})}
$$



###### Mean Square Error
___
$$MSE = (1/n) * Σ(yᵢ - ŷᵢ)²$$
___

