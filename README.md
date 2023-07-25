# cryptoclustering_challenge
Module 19 Challenge

# Before You Begin
I've created a fresh repository for this project called "CryptoClustering."

I've already cloned the repository to my computer and pushed the changes to GitHub.

# Instructions
Here's what I'll be doing in this project:

Rename the file "Crypto_Clustering_starter_code.ipynb" to "Crypto_Clustering.ipynb" for better organization.

Load the "crypto_market_data.csv" into a DataFrame.

Get the summary statistics and plot the data to get an overview of how it looks.

Prepare the Data
I'll use the "StandardScaler()" module from scikit-learn to normalize the data from the CSV file.

Create a new DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

Find the Best Value for k Using the Original Scaled DataFrame
I'll use the elbow method to find the best value for k. I'll create a list with k values ranging from 1 to 11.

I'll compute the inertia for each value of k and plot a line chart to visually identify the optimal value for k.

I'll answer the question: What is the best value for k?

Cluster Cryptocurrencies with K-means Using the Original Scaled Data
I'll initialize the K-means model with the best value for k.

I'll fit the K-means model using the original scaled DataFrame.

I'll predict the clusters to group the cryptocurrencies and add a new column to the original data to store the predicted clusters.

I'll create a scatter plot using hvPlot to visualize the clusters with "PC1" on the x-axis and "PC2" on the y-axis. I'll use different colors to represent different clusters and add the "coin_id" column in the hover to identify each cryptocurrency.

Optimize Clusters with Principal Component Analysis (PCA)
I'll use the original scaled DataFrame to perform PCA and reduce features to three principal components.

I'll retrieve the explained variance to understand the information attributed to each principal component.

I'll answer the question: What is the total explained variance of the three principal components?

I'll create a new DataFrame with the PCA data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

Find the Best Value for k Using the PCA Data
I'll use the elbow method on the PCA data to find the best value for k. I'll create a list with k values ranging from 1 to 11.

I'll compute the inertia for each value of k and plot a line chart to visually identify the optimal value for k.

I'll answer the question: What is the best value for k when using the PCA data? Does it differ from the best value for k found using the original data?

Cluster Cryptocurrencies with K-means Using the PCA Data
I'll initialize the K-means model with the best value for k.

I'll fit the K-means model using the PCA data.

I'll predict the clusters to group the cryptocurrencies and add a new column to the PCA DataFrame to store the predicted clusters.

I'll create a scatter plot using hvPlot to visualize the clusters with "price_change_percentage_24h" on the x-axis and "price_change_percentage_7d" on the y-axis. I'll use different colors to represent different clusters and add the "coin_id" column in the hover to identify each cryptocurrency.

Visualize and Compare the Results
I'll create composite plots using hvPlot and the plus sign (+) operator to compare the elbow curves and cryptocurrency clusters obtained from the original data and the PCA data.

I'll answer the question: Based on visually analyzing the cluster analysis results, what's the impact of using fewer features to cluster the data by using K-means?

Coding Conventions and Formatting
I'll ensure my code follows good coding conventions and formatting guidelines. I'll keep my code DRY (Don't Repeat Yourself) and use concise logic for maintainable and reusable code.

Deployment and Submission
For submission, I'll provide a link to my GitHub repository, where I've cloned the project files. I'll add and commit my files using the command line with appropriate commit messages.
