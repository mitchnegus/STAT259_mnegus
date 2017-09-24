# Laken, Notes

## Original Paper
-composite samples, (2) $5 \times 1$ vectors

* (2) $n \times m$ matrices
* $n = 5$: months May–September
* $m = 12$: 12 years of most precipitation ($\textbf{F}$), least precipitation ($\textbf{D}$)
* averaged in $n$ dimension $\rightarrow 5\times 1$

Used Pearson's corr. coefficients ($ r= \frac{\text{cov}(X,Y)}{\sigma_X \sigma_Y} $) to evaluate how close these vectors were to demonstrating a linear relationship between $X$ and $Y$ (month to neutron counts).

Found values of -0.95 for $\textbf{D}$ and 0.99 for $\textbf{F}$. 

Used two-tailed Student's t-test to test probability.
Found probability of $p = 0.01$ for $\textbf{D}$ and $p = 1 \times 10^{-3}$ for $\textbf{F}$. Cumalitve probability $1.4 \times 10^{-5}$ (or $1\,/\,71942$ if the null hypothesis true).

## Analysis

Took MC samples (100,000) randomly from neutron monitor data

Averaged similar to original composites

Found $r$ values. The set of 100,000 $r$ values is labeled $H_0$

This should support null hypothesis (there should be no linear relationship between randomly drawn samples)

Not what is shown, clearly the data is not Gaussian (as it would be assuming null hypothesis); the Gaussian then can't be used to calculate probabilities.

When a better logistic (or actually, even better, 4th order polynomial) fit is used the cumulative p-value is 0.91 (91% chance of occurring given null hypothesis)

