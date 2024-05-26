# About Dataset:

1. **Title: Balance Scale Weight & Distance Database**

2. Relevant Information: 
	This data set was generated to model psychological
	experimental results.  Each example is classified as having the
	balance scale tip to the right, tip to the left, or be
	balanced.  The attributes are the left weight, the left
	distance, the right weight, and the right distance.  The
	correct way to find the class is the greater of 
	(left-distance * left-weight) and (right-distance *
	right-weight).  If they are equal, it is balanced.

3. Number of Instances: 625 (49 balanced, 288 left, 288 right)

4. Number of Attributes: 4 (numeric) + class name = 5

5. Attribute Information:
	1. Class Name: 3 (L, B, R)
	2. Left-Weight: 5 (1, 2, 3, 4, 5)
	3. Left-Distance: 5 (1, 2, 3, 4, 5)
	4. Right-Weight: 5 (1, 2, 3, 4, 5)
	5. Right-Distance: 5 (1, 2, 3, 4, 5)

6. Missing Attribute Values: 
	none

7. Class Distribution: 
   1. 46.08 percent are L
   2. 07.84 percent are B
   3. 46.08 percent are R


# About Decision-Tree-Algorithm:

A decision tree is a flowchart-like structure used to make decisions or predictions. It consists of nodes representing decisions or tests on attributes, branches representing the outcome of these decisions, and leaf nodes representing final outcomes or predictions. Each internal node corresponds to a test on an attribute, each branch corresponds to the result of the test, and each leaf node corresponds to a class label or a continuous value.
Structure of a Decision Tree
1.	Root Node: Represents the entire dataset and the initial decision to be made.
2.	Internal Nodes: Represent decisions or tests on attributes. Each internal node has one or more branches.
3.	Branches: Represent the outcome of a decision or test, leading to another node.
4.	Leaf Nodes: Represent the final decision or prediction. No further splits occur at these nodes.
How Decision Trees Work?
The process of creating a decision tree involves:
1.	Selecting the Best Attribute: Using a metric like Gini impurity, entropy, or information gain, the best attribute to split the data is selected.
2.	Splitting the Dataset: The dataset is split into subsets based on the selected attribute.
3.	Repeating the Process: The process is repeated recursively for each subset, creating a new internal node or leaf node until a stopping criterion is met (e.g., all instances in a node belong to the same class or a predefined depth is reached).
Metrics for Splitting
•	Gini Impurity: Measures the likelihood of an incorrect classification of a new instance if it was randomly classified according to the distribution of classes in the dataset.
•	Gini=1–∑𝑖=1𝑛(𝑝𝑖)2Gini=1–∑i=1n(pi)2, where pi is the probability of an instance being classified into a particular class.
•	Entropy: Measures the amount of uncertainty or impurity in the dataset.
•	Entropy=−∑𝑖=1𝑛𝑝𝑖log⁡2(𝑝𝑖)Entropy=−∑i=1npilog2(pi), where pi is the probability of an instance being classified into a particular class.
•	Information Gain: Measures the reduction in entropy or Gini impurity after a dataset is split on an attribute.
•	InformationGain=Entropyparent–∑𝑖=1𝑛(∣𝐷𝑖∣∣𝐷∣∗Entropy(𝐷𝑖))InformationGain=Entropyparent–∑i=1n(∣D∣∣Di∣∗Entropy(Di)), where Di is the subset of D after splitting by an attribute.
Advantages of Decision Trees
•	Simplicity and Interpretability: Decision trees are easy to understand and interpret. The visual representation closely mirrors human decision-making processes.
•	Versatility: Can be used for both classification and regression tasks.
•	No Need for Feature Scaling: Decision trees do not require normalization or scaling of the data.
•	Handles Non-linear Relationships: Capable of capturing non-linear relationships between features and target variables.
Disadvantages of Decision Trees
•	Overfitting: Decision trees can easily overfit the training data, especially if they are deep with many nodes.
•	Instability: Small variations in the data can result in a completely different tree being generated.
•	Bias towards Features with More Levels: Features with more levels can dominate the tree structure.


