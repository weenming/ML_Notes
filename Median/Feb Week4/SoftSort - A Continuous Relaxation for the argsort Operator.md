[[Article Note]]

[PDF](files/fileDoesNotExist/notExistingFile)

## Why 
*Why did I choose to read this article to read?*

Relavent to median. In [[Reliable Graph Neural Networks via Robust Aggregation]] the [[Soft Medoid]] was realized by soft argmin

Recommended by Dr. Liu
Techniques may inspire the design of robust GNN  

## Background
*Relavent researches / the problem*


## Method


## Contribution



## Summary


## My Thoughts

But why is this differentiable? 

When $s_i$ is very close to $s_j$ the derivative does not seem to  explode when row $i$ and $j$ swaps, becasue $\mbox{softmin } \{d(s_i - s_j), 0\}$ seems to be permutable with $\mbox{softmin } \{0, d(s_j - s_i)\}$ : the sort itself is non-differentiable only at limited places and is always continuous! 

Convergence to hard sort is proved in the appendix