---
tags:
  - Evergreen/Seedling
  - statistics
  - biostatistics
  - definition
---

### Definition
___
*Principal component analysis (PCA)* is a popular technique for analyzing large datasets containing a high number of dimensions/features per observation, reducing the dimensionality of the dataset, and increasing the interpretability of data while preserving the maximum amount of information, and enabling the visualization of multidimensional data.

**(Alt.)** *Principal Component Analysis (PCA)* takes a large data set with many variables per observation and reduces them to a smaller set of summary indices.

It does so by mapping the data to a new plane (see Image):

![[Pasted image 20230912130155.png | center-align]]

##### Example use cases
- In Machine Learning, *PCA* is used to visualize multidimensional data.

- *PCA* can help resize an image for medical studies, analyze stock data and forecast future data.
___

## Video explanations

![PCA by Washington University](https://www.youtube.com/watch?v=fkf4IBRSeEc&ab_channel=SteveBrunton)


![PCA by StatQuest](https://www.youtube.com/watch?v=FgakZw6K1QQ&ab_channel=StatQuestwithJoshStarmer)



## Formulae
The k-th principal component of a data vector x(i) can therefore be given as a score $t_{k(i)} = x_i ⋅ w_k$ in the transformed coordinates, or as the corresponding vector in the space of the original variables, {$x_i ⋅ w_k$} $w_k$, where $w_k$ is the k<sup>th</sup> [[eigenvector]] of X<sup>T</sup>X.

(Also see notes on [[Singular Value Decomposition (SVD)]], which is used in PCA)












