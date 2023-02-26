
Metric of robustness: [[Breakdown Point]]

## Marginal Median

Dimension-wise median, I think is equivalent to minimizing sum of $l_1$ norm 

problem:

> The fundamental problem is that the point whose coordinates are the marginal medians can be located unreasonably far from _any_ data values (or probability).

![[Pasted image 20230223023920.png]]

## Geometric Median
$l_2^1$ median, [WikiPedia]([Geometric median - Wikipedia](https://en.wikipedia.org/wiki/Geometric_median)) 

$$
\mbox{argmin}_{x} \sum_i\|x_i - x\|_2
$$

## Oja's Simplex Median

-   for every subset of _p_ points from the data set, form a simplex with _X_.
-   sum together the volumes of each such simplex.
-   the Oja simplex median is any point X* in Rp for which this sum is minimum.

Not in much use though

## Convex Hull Trimming



## Trimmed Median

in 1D, trimmed median is the same as the original median


## Ref
[Blog]([Robust Estimators of Location (mcgill.ca)](http://cgm.cs.mcgill.ca/~athens/Geometric-Estimators/L1med.html))