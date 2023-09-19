
___
> Author: <span class="name">Sam Hurenkamp</span>
> Tags: #Evergreen/Seedling #biostatistics #statistics #lecture
> Last modified: `$= dv.current().file.mtime`

<div class="f-info">
	<div class="course-code">
		<span class="fheader"> Course Code </span> <br/>
		<span class="fbody"> 1MB465 </span>
	</div>
	<div class="discipline">
		<span class="fheader"> Discipline </span> <br />
		<span class="fbody"> Statistics </span>
	</div>
	<div class="date">
		<span class="fheader"> Created</span> <br />
		<span class="fbody last-modified"> 2023-09-01 </span>
	</div>
</div>
___

## Topics covered
- Natural population vs statistical population vs statistical sample
- Biological variation
- Phenotypic plasticity
- Interspecific variation > intraspecific variation
- Population sampling techniques (And the pros and cons of each)
- Gaussian (normal) distribution
- Arithmetic mean 
	- population mean/sample mean
- Median
- Mode 
	- most likely value, the same as the mean in a normal distribution)
- Variance
-  Population Variance
$$
\sigma^2 = \frac{\displaystyle\sum_{i=1}^{n}(x_i - \mu)^2} {n}
$$

 -  Sample variance – unbiased
$$
s^2 = \frac{\displaystyle\sum_{i=1}^{n}(x_i - \bar{x})^2} {n-1}
$$
- Sample variance – biased
$$s_N = \sqrt {\frac{1}{N}\sum\limits_{i = 1}^N {\left( {x_i - \bar x} \right)^2 } }$$
 
 - Standard deviation in population/sample ($Z$<sub>pop</sub>/$Z$<sub>sample</sub>)
	$𝜎$ = $𝜎^2$ and $𝑠$ = $𝑠^2$

$$
Z_{𝑝𝑜𝑝} = \frac{(𝑥 − 𝜇)}{𝜎} 
$$
$$
Z_{sample} = \frac{(x-\bar{x})}{s}
$$


### **The Central Limit Theorem** 
> [Probability Demonstration: The Galton Board](https://www.youtube.com/shorts/TwctT3Ncm1w)

```
The central limit theorem (CLT) **states that the distribution of sample means approximates a normal distribution as the sample size gets larger, regardless of the population's distribution**. Sample sizes equal to or greater than 30 are often considered sufficient for the CLT to hold
```

- Standard error of the mean (SEM)
$$
SEM = \frac{s} {\sqrt{n}} = \sqrt{\frac{s^2}{n}}
$$

- Type I and Type II errors

- Statistical power
1-β, the probability to reject H<sub>0</sub> when H<sub>A</sub>

___
*β is the type II error!*
___

## Statistical Power
___
$$
Power ∝ \frac{E α \sqrt{n}}{σ}
$$
E = Effect Size
α = probability of a Type I error
n = sample size
σ = standard deviation
___

> The “Effect size” is the difference in group means or the strength of a relationship between two tested variables


<b><u>Additional sources of variation</u></b>
- Random measurement error (“unproblematic”)
- Bias (systematic and more problematic)
- Contamination (nothing stats can do about this)


# Replication
![[Pasted image 20230901113231.png]]

![[Pasted image 20230901120202.png]]

