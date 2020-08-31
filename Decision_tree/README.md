**Decision Tree:**

Decision Trees ( DTs) are a non-parametric, supervised method of classification and regression learning. The aim is to build a model that predicts the value of a target variable by learning from the data features basic decision rules. For example , decision trees learn from data about approximating a sine curve with a set of if-then-else decision rules. The larger the vine, the more complicated the rules governing the decision and the fitter the model.
DecisionTreeClassifier takes two arrays as its input: an array X, sparse or dense, of size [n samples, n features] holding the training samples, and an array Y of integer values, size [n samples] holding the training sample class labels.


The __advantages__ of decision trees are:
1) Easy to understand and interpret. Trees can be visualized.
2) Requires little preparation of the results. Other strategies also involve data normalisation, generating dummy variables and eliminating blank values. Remember that this module does not support missing values, however.
3) The cost of using the tree (i.e., predicting data) in the number of data points used to train the tree is logarithmic. 
4) Performs well even if its assumptions are somewhat in breach of the true model from which the data was generated.

The __disadvantages__ of decision trees include:
1) Decision-tree learners can create over-complex trees that do not generalise the data well. This is called overfitting. Mechanisms such as pruning, setting the minimum number of samples required at a leaf node or setting the maximum depth of the tree are necessary to avoid this problem.Decision trees can be unstable because small variations in the data might result in a completely different tree being generated. This problem is mitigated by using decision trees within an ensemble.
2) It is known that the problem of learning an optimal decision tree is NP-complete under several aspects of optimality and even for simple conceptions. Practical decision-tree learning algorithms are also based on heuristic algorithms such as the greedy algorithm, where optimal decisions are made locally at each node. These algorithms can not guarantee that the decision tree which is globally optimal would return. It can be mitigated by training several trees in a learner ensemble, where the features and samples are sampled randomly with replacement.
3) There are concepts that are difficult to understand, as decision trees can not easily articulate them, such as difficulties with XOR, parity or multiplexer.
4) Learners from decision-making tree build biased trees when other groups dominate. Therefore, it is recommended that the dataset be balanced before integrating with the decision tree.
