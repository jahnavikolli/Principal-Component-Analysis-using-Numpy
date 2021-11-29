# Principal-Component-Analysis-using-Numpy

In this course, we are going to focus on three learning objectives:

1. Implement Principal Component Analysis (PCA) from scratch with NumPy and Python
2. Conduct basic exploratory data analysis (EDA)
3. Create simple data visualizations with Seaborn and Matplotlib

By the end of this course, you will be able to implement all the machine learning without using any of the popular machine learning libraries such as scikit-learn and statsmodels so you have a deeper understanding of the fundamentals.

Course Structure
This course is divided into 3 parts:

# The hands on project on Principal Component Analysis with NumPyis divided into following tasks:



**Task 1: Load the Data and Import Libraries**

1. Load the dataset using pandas.
2. Import essential modules and helper functions from NumPy and Matplotlib.
3. Explore the pandas dataframe using the head() and info() functions.


**Task 2: Visualize the Data**

1. Before starting on any task, it is often useful to understand the data by visualizing it.
2. For this dataset, we can use a scatter plot using Seaborn to visualize the data.


**Task 3: Data Standardization**

1. With great power to reduce dimensionality, comes great responsibility.
One must take care to preprocess the input data appropriately.
2. Make sure to zero-out the mean from each feature (subtract the mean of each feature from the training set), and normalize the values if your features have differing units.
3. PCA is best used when the data is linear, because it is projecting it onto a linear subspace spanned by the eigenvectors.
4. This is an important step in many machine learning algorithms, and especially so in the case of PCA. We want the PCA algorithm to give equal weight to each of the features while making the projection.
5. If one or more features are in a different scale than the rest, those non-standardized features will dominate the eigenvalues and give you an incorrect result This is a direct consequence of how PCA works. It is going to project our data into directions that maximize the variance along the axes. 


**Task 4: Compute the Eigenvectors and Eigenvalues**

1. There are two general ways to perform PCA. The more computationally effective way is to do something called Singular Value Decomposition or SVD.
2. It decomposes a matrix into the product of two unitary matrices (U, V*) and a rectangular diagonal matrix of singular values (S).
3. The mathematics of computing the SVD is a little complicated and out of the scope of this project. If you’re familiar with linear algebra, I highly encourage you to read about it on your own time.
4. Luckily for us, there is a numpy function that performs SVD on the input matrix, so we don’t really need to worry about the math for now.
5. We’re going to cover SVD in the next task.
6. Recall that PCA aims to find linearly uncorrelated orthogonal axes, which are also known as principal components (PCs) in the m dimensional space to project the data points onto those PCs. The first PC captures the largest variance in the data.
7. The PCs can be determined via eigen decomposition of the covariance matrix Σ. After all, the geometrical meaning of eigen decomposition is to find a new coordinate system of the eigenvectors for Σ through rotations.


**Task 5: Singular Value Decomposition (SVD)**

1. Singular Value Decomposition or SVD is a computationally efficient method to perform PCA.
2. It decomposes a matrix into the product of two unitary matrices (U, V*) and a rectangular diagonal matrix of singular values (S). The mathematics of computing the SVD is a little complicated and out of the scope of this project.


**Task 6: Selecting Principal Components Using the Explained Variance**

1. The use of PCA means that the projected data can be analyzed along axes of principal variation.
2. Plot the cumulative explained variance against the number of principal components.
3. Rank components according to the explained variance each component contributes to the model.


**Task 7: Project Data Onto Lower-Dimensional Linear Subspace**
Utilize principal component analysis to decompose high dimensional data into two or three dimensions so that each instance can be plotted in a scatter plot.
