[[Article Note]]
[[Adverserial Attack]] [[Soft Medoid]] [[Reliable Graph Neural Networks via Robust Aggregation]]
[PDF](files/)

## Why 
*Why did I choose to read this article?*

Recommended by Dr. Liu; covers many new works on adversarial attack on GNN; potential new framework for defense.



## Background
*Relavent researches*

### Common Attacks
- Aim: misclassification of
	- Global
	- Single node
- Descent scheme
	- greedy attacks
	- Projected Gradient Descent (PGD)
- When to attack
	- Evasion
	- Poisoning

### Defenses
Characterization
![[Pasted image 20230226201036.png]]


### Evaluation

Traditionally, robustness is evaluated as follows:
	Optimize *adversarial attack* w.r.t. vanilla GCN but test on modified model.

What should be done: 
	Design attack for each defense s.t. the attack can be optimized for the defense


## Method

General rule to design adaptive attacks: if defferentiable, use gradient-based methods directly on the defense model, else PGD?

Before adaptive, a new model should first pass the standarized, black-box "unittests".

#### SVD-GCN

#### ProGNN

#### Soft Median
In supp. E.7
So for dim-wise median, add new edges? 


## Contribution
*The problem that this work solves*



## Summary


## My Thoughts