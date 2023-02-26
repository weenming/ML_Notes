
## Background
Classification tasks:
- classification error
- MSE -> slow learning rate at the beginning
- CE


## Method

For **one** data point to classify (a image in NN, a node in GNN etc.), define the probability density of the prediction as $p(x)$ and true (label) distribution as $q(x)$. The CE loss is given as 
$$
L = -\int_x q(x) \log(p(x)) dx
$$
E. g., in the n-classification task, $L=-\sum_i^N q_i\log p_i$ , where $q_i = \delta_{ii_0}$ and thus $L = -\log p_{i_0}$ . At optimzal condition $p_{i_0} = 1$,  $L$ is minimized.

The merit function of the model can be simply added up across different samples.