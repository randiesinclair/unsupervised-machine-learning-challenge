# Unsupervised Machine Learning challenge

In this exercise, I am a member of a data science team in a medical research company. Our current focus is on finding ways to improve the prediction of nearsightedness, also known as myopia. Despite our attempts to enhance our classification model using the entire dataset, we have been unsuccessful. 

However, we believe that analyzing distinct groups of patients separately might be more effective. My supervisor has tasked me with exploring this possibility using unsupervised learning. 

To begin, I will need to process the raw data to fit our machine learning models. After that, I will use various clustering algorithms to group patients and determine if they can be categorized into distinct groups. Finally, I will create a visualization to share my findings with my team and other stakeholders.

# Technical Skills
- Unsupervised Machine Learning
- Pandas
- Standardization of dataset
- PCA (Principal Component Analysis)
- t-SNE (t-Distributed Stochastic Neighbor Embedding)
- K-means clustering algorithm for performing a cluster analysis
- Elbow plot creation

# Parameters
### Data Preparation
- Reads the csv into pandas
- Previews the DataFrame
- Removes the MYOPIC column from the dataset
- Standardizes the dataset using a scaler
- Names the resulting DataFrame X

<img src="Resources/code%20snapshots/Capture1.JPG" width="50%" height="50%">

### Dimensionality Reduction
- PCA model is created and used to reduce dimensions of the scaled dataset
- PCA model’s explained variance is set to 90% (0.9)
- The shape of the reduced dataset is examined for reduction in number of features

![Alt text](Resources/code%20snapshots/Capture2.JPG)

- t-SNE model is created and used to reduce dimensions of the scaled dataset
- t-SNE is used to create a plot of the reduced features

![Alt text](Resources/code%20snapshots/Capture3.JPG)

### Clustering
- A K-means model is created
- A for- loop is used to create a list of inertias for each k from 1 to 10, inclusive
- A plot is created to examine any elbows that exist

![Alt text](Resources/code%20snapshots/Capture4.1.JPG)

<img src="Resources/code%20snapshots/elbowCurveViz.JPG" width="70%" height="40%">

- States a brief (1-2 sentence) conclusion on whether patients can be clustered together, and supports it with findings

![Alt text](Resources/code%20snapshots/Capture4.2.JPG)

<img src="Resources/code%20snapshots/ClusterViz.JPG" width="70%" height="40%">