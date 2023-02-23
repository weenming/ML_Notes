[[Article Note]]

[PDF](files/Average/RobustnessOfGraphNeuralNetworksAtScale_NeuralIPS.pdf)

## Background
*Relavent researches*
Existing research: small graphs -> this work: adverserial attacks on GNN at scale [[GNN]] [[At Scale]] and the defense [[Adverserial Attack]]

[[Surrogate Loss]]es are not suitable for global attacks [[To Learn]]

New robust [[Aggregation Function]]: [[Soft Meadian]] 


## Method

### Surrogate losses for global attacks

Problem of [[Corss Entropy]] methods: conventionally ([[To Learn]]) an attack maximizes the average CE, but this tends to attack unimportant nodes (i.e. those already misclassified) and thus waste the budget.

The accuracy should be used to determine the importance of a certain *node*. CE is used in training because training does want to optimize the misclassified nodes.

[[To Learn]] How do 'local' attacks choose what nodes to attack: maximize CE by defining some loss to minimize? should not be like this because it is not "local"

### Attack


### Scalable Defense

Soft-Median at aggregation
Best possible [[Breakdown Point]]    [[To Learn]]
Outperforms [[Soft Medoid]] in [[Reliable Graph Neural Networks via Robust Aggregation]] and also its *hard equivalent*. 

Aproach: weighted mean according to the $l_2$ distance to the *[[Dimension-wise Mean]]* 
$$
\mu_{WSM}(X, a)=-C x^T \mbox{ softmin }({\|\bar{x} - x\|_2 \over T\sqrt{d}})
$$
where $d$ is dimension, $T$ is a hyperparameter and $C$ is the normalization factor s.t. $\sum \mu_{WSM} = \sum x$.
Converges to mean when $T\rightarrow \infty$ and hard dimension-wise median.

## Contributions
*The problem that this work solves*

Adverserial attacks on large scale GNN

## Summary

- Surrogate Loss: limitation of the state-of-art surrogate loss
- Attack: Novel attack technique of attacks on GNNs which saves memory [[Adverserial Attack]]
- Defense: soft median, computationally efficient aggregation at scale, using soft sorting


## My Thoughts
 
So does the [[Dimension-wise Mean]] have any shortcoming?