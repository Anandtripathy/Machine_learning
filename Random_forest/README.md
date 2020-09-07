# Random Forest 

In random forests (see RandomForestClassifier and RandomForestRegressor classes), each tree in the ensemble is constructed from a sample drawn from the training set with replacement (i.e., a bootstrap sample).Moreover, when splitting each node when constructing a tree, the best split is found either from all input features or from a random subset of max features size.
These two sources of randomness have the effect of decreasing the forest estimator variance. Usually, individual decision trees show high variance and appear to overfit. The randomness introduced into the forests yields decision trees with somewhat decoupled predictive errors. Many mistakes may be eliminated, by taking an average of those predictions. By combining diverse trees, random forests achieve a reduced variance, sometimes at the cost of a slight increase in bia. In practise the reduction in variance is always important, resulting in a stronger overall model.

**Advantages of Random Forest:**

1)  Random Forest is based on the bagging algorithm and uses Ensemble Learning technique. It creates as many trees on the subset of the data and combines the output of all the trees. In this way it reduces overfitting problem in decision trees and also reduces the variance and therefore improves the accuracy.

2) Random Forest can be used to **solve both classification as well as regression problems.**

3)  Random Forest works well with both **categorical and continuous variables.**

4) **Handles non-linear parameters efficiently:** Non linear parameters don't affect the performance of a Random Forest unlike curve based algorithms. So, if there is high non-linearity between the independent variables, Random Forest may outperform as compared to other curve based algorithms

**Disadvantages of Random Forest:**

1) **Complexity:** Random Forest creates a lot of trees (unlike only one tree in case of decision tree) and combines their outputs. By default, it creates 100 trees in Python sklearn library. To do so, this algorithm requires much more computational power and resources. On the other hand decision tree is simple and does not require so much computational resources.

2) **Longer Training Period:** Random Forest require much more time to train as compared to decision trees as it generates a lot of trees (instead of one tree in case of decision tree) and makes decision on the majority of votes.
