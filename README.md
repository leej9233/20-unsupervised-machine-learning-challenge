# 20-unsupervised-machine-learning-challenge

Background
You are on the data science team of a medical research company that’s interested in finding better ways to predict myopia, or nearsightedness. Your team has tried—and failed—to improve their classification model when training on the whole dataset. However, they believe that there might be distinct groups of patients that would be better to analyze separately. So, your supervisor has asked you to explore this possibility by using unsupervised learning.

You have been provided with raw data, so you’ll first need to process it to fit the machine learning models. You will use several clustering algorithms to explore whether the patients can be placed into distinct groups. Then, you’ll create a visualization to share your findings with your team and other key stakeholders.

# Instructions
This activity is broken down into four parts:

Part 1: Prepare the Data.

Part 2: Apply Dimensionality Reduction.

Part 3: Perform a Cluster Analysis with K-means.

Part 4: Make a Recommendation.

# Part 1: Prepare the Data
Read myopia.csv into a Pandas DataFrame.

Note: This file can be found in your Module 20 Challenge files.
Remove the "MYOPIC" column from the dataset.

Note: The target column is needed for supervised machine learning, but it will make an unsupervised model biased. After all, the target column is effectively providing clusters already!
Standardize your dataset so that columns that contain larger values do not influence the outcome more than columns with smaller values.

# Part 2: Apply Dimensionality Reduction
Perform dimensionality reduction with PCA. How did the number of the features change?

HINT
Further reduce the dataset dimensions with t-SNE and visually inspect the results. To do this, run t-SNE on the principal components, which is the output of the PCA transformation.

Create a scatter plot of the t-SNE output. Are there distinct clusters?

# Part 3: Perform a Cluster Analysis with K-means
Create an elbow plot to identify the best number of clusters. Make sure to do the following:

Use a for loop to determine the inertia for each k between 1 through 10.

If possible, determine where the elbow of the plot is, and at which value of k it appears.

# Part 4: Make a Recommendation
Based on your findings, write up a brief (one or two sentences) recommendation for your supervisor in your Jupyter Notebook. Can the patients be clustered? If so, into how many clusters?
