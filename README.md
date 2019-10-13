# Black-Friday-Prediction
This is my approach on Analytics Vidhya Black Friday hackathon. You can find a complete step-by-step analysis on the issue as well as my Python code and conclusions.

**Problem Statement**  <br />
The challenge was to predict purchase prices of various products purchased by customers based on historical purchase patterns. The data contained features like age, gender, marital status, categories of products purchased, city demographics etc.

# Machine Learning Project Checklist
My machine learning project workflow mainly includes the following parts and it also shows how I tackle this series of problems. Suppose we get the dataset, then start our journey and let the data lead us and see what information could we get and how to accomplish the task.

**Frame the Problem** <br />
1. Specify business objective.<br />
2. Transform the problem that can be addressed using data and ML algorithms.<br />
   (Supervised/Unsupervised, classification/regression/clustering, online/offline, etc.)?<br />
   
The right set up is often more important than the choice of algorithm. Make sure you are solving the right problem.

**Get the Data** <br />

Build robust dataset to solve real-world problems and see how your data preparation ultimately impacts how effective you models are.<br />

1. List the data you need and how much you need.<br />
2. Try to collect the data and check the size and type of data.<br />
3. Some problems you might meet like imbalanced data. <br />
4. Sample a test set and never touch it until last moment.<br />

**Explore the Data**
1. Study each attribute and its characteristics: Name, Type, % of missing values, Noisiness, Type of distribution, etc.
2. Visualize the data involving a bunch of plot.
3. Study the correlations between variables.
4. Identify the promising transformations you may want to apply.
5. Gain insights for feature engineering. 

**Prepare the Data**
1. Data cleaning: <br />

    (1) Fix or remove outliers.<br />
    (2) Fill in missing values or drop their rows or columns.<br />
  
2. Feature selection <br />
More features may not lead to a better-fitted model. Pay attention to the curse of dimensionality. If needed, drop the features that provide no useful information for the task. <br />

3. Feature engineering <br />

  Building better features is after data, the second most important way to impact Machine Learning performance. Feature        engineering is how we take our knowledge about the world and encode it into a format that our model can leverage          effectively. Coming up with new features is difficult and time-consuming, it needs domain knowledge or familiarity with your dataset. However, deep learning blurs the difference between the features and the model. In general, feature engineering includes:

   (1) Discretize continuous features <br />
   (2) Decompose features like categorical, date/time, etc. <br />
   (3) Add promising transformations of features like log(x), sqrt(x), x^2, etc.<br />
   (4) Aggregate features into promising new features.<br />
  
4. Feature scaling: standardize or normalize features. <br />

5. Partition data. According to your concrete situation, split the dataset into train, validation and test set. Make sure every set should work properly.

**Evaluate Model Performance**

For a specific task, we have various metrics as candidates like accuracy, error, AUC or F score. Choosing the most proper one that helps us identify what it means to be successful and how to measure it. The metric should be consistent with your business goal or your task. <br />

**Short-List Promising Models**

1. Train many quick and dirty models from different categories using standard parameters.

2. Measure and compare their performance.

3. Analyze the most significant variables for each algorithm.

4. Analyze the types of errors the models make.

5. Have a quick round of feature selection and engineering.

6. Have one or two more quick iterations of the five previous steps.

7. Short-list the top three to five most promising models, preferring models that make different types of errors.

  Ideally, features and data should govern model choice. A good understanding of statistical learning and the fundamentals of the different algorithms can help make the choice naturally, but we also need to think about tradeoffs. For model, sole     objective is reducing the loss on the test set as far as possible. For the real world, a few areas we should think about are: interpretability and ease to debug, data volume, and training and prediction considerations.

**Fine-Tune the System**

1. Fine-tune the hyperparameters using cross-validation with Random search or Grid search. Hyperparameters are not only about models but also about your data transformation choices, especially when you are not sure about them. For example, the way you treat missing values or converting formats you use.

2. Try ensemble methods. Ensemble can usually boost performance and often perform better than running them individually. But be observant of making the tradeoff between precise prediction and time cost.

3. Measure the final model on the test set to estimate the generalization error.
 
