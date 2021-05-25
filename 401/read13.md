# How to run Linear regression in Python Scikit-learn 
 Scikit-learn is a powerful Python module for machine learning. It contains function for regression, classification, clustering, model selection and dimensionality reduction. Today, I will explore the sklearn.linear_model module which contains “methods intended for regression in which the target value is expected to be a linear combination of the input variables”.

 The first step is to import the required Python libraries into Ipython Notebook.

 ![Explore 1](https://bigdata-madesimple.com/wp-content/uploads/2016/04/Explore-1.png)

 This data set is available in sklearn Python module, so I will access it using scikitlearn. I am going to import Boston data set into Ipython notebook and store it in a variable called boston.

 ## Scikit Learn
 In this section I am going to fit a linear regression model and predict the Boston housing prices. I will use the least squares method as the way to estimate the coefficients.

 Y = boston housing price(also called “target” data in Python)

 and

 X = all the other features (or independent variables)
