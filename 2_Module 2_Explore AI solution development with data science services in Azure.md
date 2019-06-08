# Module 2: Explore AI solution development with data science services in Azure



# PART 1: Introduction to Data Science in Azure

# Introduction

- 5 minutes

In recent years, the term *data science* has become more popular due to the influx of data in all areas of business. Data science is about getting valuable insights from information, and answering questions by analyzing data using statistical methods, computing power, and automation.

One of the core concepts behind data science is using historical data to predict the future. To do this, you use data values you know to predict something you don't know. However, this requires that you have historical data with the outcome you want to predict and other data that correlates to this outcome. For example, let's say you want to predict the likelihood a person will default on a loan. If you have data points for a history of loans that were repaid versus those that defaulted, and their corresponding data such as income, employment status, and credit rating you can define a model to help predict loan defaults.

Other examples include predicting a technological problem occurring, or trying to understand the patterns in types of products customers are buying. As you can see, the types of questions that can be answered through data science vary greatly.

Data science is based on probabilities. So along with getting predicted outcomes, the estimated probability of the outcome is a critical consideration. A business is looking to answer a data-driven question often follow a set of predefined steps known as the *data science process*.

## Learning objectives

In this module, you will:

- Learn the steps involved in the data science process
- Learn the machine learning modeling cycle
- Learn data cleansing and preparation
- Learn model feature engineering
- Learn model training and evaluation
- Learn about model deployment
- Discover the specialized roles in the data science process

------

## Next unit: The Data Science process

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-science-in-azure/2-data-science-process)









# The Data Science process

- 5 minutes

It's easy to get lost in the data science process because there can be several components in each step. However, the process stays the same regardless of the type of the problem that is trying to be solved. Let's begin by defining each step and use an example to understand what each step would look like.

Let's say you work for a company that sells a variety of products ranging from clothes to groceries and cleaning products. Management noticed they were running out of brooms before the end of each month. They wanted to solve this problem, so they decided to hire your team to help them build a solution.

![Screenshot of Data Science Solution Framework](https://docs.microsoft.com/en-us/learn/data-ai-cert/intro-to-data-science-in-azure/media/2-solution-framework.png)

## Understand the business problem

In any problem-solving method the problem must first be identified. This can either be in the form of a question or a statement. There is always a general business understanding that will motivate the data science process in each situation.

In our example, your company understands they could be selling more brooms if they knew how many they could expect to sell each month, and stock their shelves accordingly.

## Understand and prepare the data

Data understanding comes from the process of acquiring and exploring available data. This step involves obtaining and preparing the data to be used in model training. To train models, it's important to understand the data. Data scientists start by performing exploratory data analysis (EDA) to better understand the data they're working with, and identify which data elements drive the outcome they want to predict. With this understanding, can cleanse the data and extract the features required for modeling.

Your company gives their data to the data science team. The data engineer cleans and preps the data so that it's ready for the modeling process. EDA helps you learn about the relationship among data elements, which helps determine which data (or *features*) you will need to train the model. For example, it might help to know what people most frequently buy with brooms.

## Model the data

The modeling step is a cycle of steps that occur to improve results. (This cycle will be explained more in depth in the following unit) Modeling can consist of several techniques, but typically one cycle iteration is not enough to produce good results, so the cycle is repeated until the desired results are achieved.

You use the available data and move into modeling and feature engineering. For this type of question where there are many different numerical variables, you try a time series model and evaluate its performance.

## Deployment

This step is usually left to the developers. It consists of integrating the solution into the business to solve the original problem. For your company, deployment would mean using the prediction of broom sales to properly stock the shelves.

## Summary

Data science is a data-driven process that starts with a question. Data acquisition and understanding then drives the modeling. The steps a data scientist usually focuses on are data understanding and modeling, which is where the results are produced. After that, the developer implements the results to test the performance.

------

## Next unit: What is modeling?

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-science-in-azure/3-what-is-modeling)







# What is modeling?

- 5 minutes

When people think of the role of a data scientist they often correlate it with machine learning modeling, which is a procedure that takes place within the data science process. In this phase, the data scientist uses EDA, feature engineering, and modeling to give a probabilistic outcome based on the data at hand.

## Understand the cycle

The modeling step is often a cycle of data understanding, feature engineering, modeling, and model evaluation. Each of the steps in the modeling cycle can take a significant amount of time. A common misconception is that the modeling step alone is data science, but the reality is each of the components of the process are vital.

![Screenshot of the modeling cycle.](https://docs.microsoft.com/en-us/learn/data-ai-cert/intro-to-data-science-in-azure/media/3-modeling-cycle.png)

Later in the module we will discuss each of the steps of the cycle, but first, let's review the cycle itself.

## Exploratory Data Analysis (EDA)

Exploratory Data Analysis (EDA) can be an extremely useful step. Often, this part of the cycle will give insight into what needs to be done during feature engineering and modeling to produce the best results. You can use different techniques depending on the types of data you are working with. A few common visualization techniques are histograms, distribution plots, box plots, and heat maps.

## Feature engineering

Feature engineering is a large part of the modeling procedure. Creating features using the data available often goes hand in hand with EDA because when you create a feature, it's important to see how it relates to the rest of the data. Therefore, you may find yourself going back and forth between EDA and feature engineering.

Some techniques used in feature engineering are moving averages and different types of aggregations. A *moving average*is the change in average for a specific constant time interval. *Aggregations* are combinations of the data based on another feature. Some examples of aggregations are sum, average, and count.

## Modeling

A *model* is an algorithm that learns information about the data and then provides a probabilistic prediction. Creating models is the portion of the cycle that gets the most recognition. Here there are many different techniques available, so it's important to identify the type of problem being solved.

Based on the what you're predicting, you can use either the classification algorithm or the continuous value prediction algorithm. A *classification algorithm* predicts discrete values, and the *continuous value prediction algorithm* predicts continuous values.

To classify something, the only options are models that are based on that assumption. Some examples of classification models are logistic regression and random forest classifier. The outcome predicted by a classification model is finite-it must be one of a predefined set of values. This is because continuous values are numeric and can take on an infinite number of possible values. For example, in theory, total goods sold is infinite and includes a decimal portion. In reality, factors such as number of goods produced, and number of customers constrain the range of the value. However, it is still considered continuous.

## Evaluate the model

Evaluating the model allows us to see how and where the model is doing well and/or failing. This step helps you focus in on the best model for your data. There are a few different methods that are useful depending on the type of predictive algorithm you're using. If you have a classifier model it's important to use a confusion matrix to identify misclassifications using precision and accuracy. If you are predicting numerical values, you can use evaluation metrics such as mean squared error to see on average how far away the predicted values are from the true values.

![Screenshot of RMSE visualization.](https://docs.microsoft.com/en-us/learn/data-ai-cert/intro-to-data-science-in-azure/media/3-rmse.png)

## Summary

The primary role of a data scientist is performing the model cycle tasks. The cycle always begins at EDA, but the movement from there varies depending on the data. It's common to iterate through this cycle multiple times before being satisfied with the results. At the end of this cycle, other questions may arise, creating another opportunity.

------

## Next unit: Choose a use case

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-science-in-azure/4-choose-use-case)









# Choose a use case

- 5 minutes

The first step in the data science process is choosing a use case. This step is also commonly referred to as *the business understanding* because it's where a business defines their objectives and business problems. Together, the data science team and the company (stakeholders and employees) set goals and targets for the project. Generally, this is also where they identify the scope of the project.

## Identify the problem

There are many different types of questions that can be solved by data science. Examples include disease insights, sales forecasts, and hardware failures. A company that comes across a question that's answerable with data might decide to bring in a data science team to solve the problem.

In the example of your company, the business problem is that the brooms are selling out before the end of the month. Therefore, the company is looking to stock brooms according to the prediction of broom sales.

## Define the project goals

Defining the project goals and objectives begins with asking relevant and specific questions to understand the scope of the project. Your company wants to resolve their issue with broom sales, but the scope of the project must be defined first. Within the range of the project, the company and your data science team must set goals and objectives such as identifying a deadline and milestones for the project.

## Identify data sources

Most companies have a tremendous amount of data, so it's essential to decide what kind of data is necessary for the project. Then you must determine where it's stored and how to gain access to it. Depending on where the company stores the data, it is typically the data engineers' job to retrieve the data from company's data source, cleanse the data, and then deliver it to the data scientist.

## Summary

Choosing a use case allows the data scientist and their team to work with their company or client to define the objectives for the project. Gaining a business understanding encompasses identifying the problem or question, and what solving the problem may require. This part of the data science process helps all people on the data science team understand their role within the project, and identify the measures for success.

------

## Next unit: Data preparation

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-science-in-azure/5-data-preparation)









# Data preparation

- 5 minutes

Data preparation is a broad term that encompasses the beginning stages of getting the data to the point at which it's ready for modeling. This step is the responsibility of both the data engineer and the data scientist. The data engineer does most of the data preparation by making the data accessible, clean, and ready for the data scientist to work with. However, most data scientists still need to do large amount of data cleansing.

Let's focus on the portion of this process that pertains to the data scientist.

Using the example from the previous page, we know that your company has stores that sell products such as clothing, cleaning supplies, and groceries. Management has noticed that they are selling out of brooms before the end of the month, and they want to know how many brooms they should stock so they don't sell out.

The following table displays sales data from your company.

| SaleID  | ItemID | ItemName    | ItemPrice | TotalPrice | Timestamp           |
| :------ | :----- | :---------- | :-------- | :--------- | :------------------ |
| 1739283 | 1435   | Broom       | 14.99     | 20.98      | 10-02-2009 13:20:22 |
| 1739283 | 1923   | Bleach      | 5.99      | 20.98      | 10-02-2009 13:20:22 |
| 1739101 | 1435   | Broom       | 14.99     | 24.72      | 10-02-2009 20:45:38 |
| 1739101 | 1981   | Ground beef | 6.74      | 24.72      | 10-02-2009 20:45:38 |
| 1739101 | 1722   | Bananas     | Null      | 24.72      | 10-02-2009 20:45:38 |

Let's note some things about the data:

- The first two rows are referring to the same sale. Therefore, you know that this person bought a broom and bleach together.
- The last three rows are from a customer who bought a broom, ground beef, and bananas in the evening.

## Clean the data

Generally, the kinds of cleansing a data scientist will do involves null or absent values. Data that has been prepped by a data engineer won't have much cleansing left. Note that there are other names for this process.

In the previous table, you can see there is one null value for the ItemPrice for bananas. It's likely that in a large data frame, where there is one null value there are others. Therefore, to find (or *extract*) the missing ItemPrice of that item you could subtract the sum of the other ItemPrices from the TotalPrice of the same customer sale.

## Expose the data with EDA

The Exploratory Data Analysis (EDA) part of the process is crucial because of the information unveiled during this step. EDA allows for the investigation of what is happening in the data that is not obvious at a glance. Sometimes it's possible to uncover patterns within the data, build questions about the data, and reject or accept the original hypotheses about the data.

As you can see in the data from your company, you don't have a lot of features; this is not unusual. So, for your company's EDA you might want to look at the TotalPrice distribution, where ItemName is 'broom' to show patterns in people's spending when they're buying a broom. You might also want to look at the broom sales over time to see if there is a trend or seasonality to the data. These are just a few of many things you could do to understand the data.

## Summary

Although most data preparation is outside the data scientist's role, it's still imperative to understand the transformations that can be done to data. Data cleansing and EDA are vital to the modeling process, so it should never be overlooked.

------

## Next unit: Feature engineering

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-science-in-azure/6-feature-engineering)









# Feature engineering

- 5 minutes

Creating features is often an instrumental part of the process in the modeling procedure. Feature engineering allows you to extract a new feature from the original data using different methods. This technique can help you improve your model results and help you see patterns in the data that may not have been visible with the original dataset. An example of feature engineering from a datetime column is creating a separate feature based on the time of the day to add attention to it.

Your company's sales data table includes the following sales information.

| SaleID  | ItemID | ItemName    | ItemPrice | TotalPrice | Timestamp           |
| :------ | :----- | :---------- | :-------- | :--------- | :------------------ |
| 1739283 | 1435   | Broom       | 14.99     | 20.98      | 10-02-2009 13:20:22 |
| 1739283 | 1923   | Bleach      | 5.99      | 20.98      | 10-02-2009 13:20:22 |
| 1739101 | 1435   | Broom       | 14.99     | 24.72      | 10-02-2009 20:45:38 |
| 1739101 | 1981   | Ground beef | 6.74      | 24.72      | 10-02-2009 20:45:38 |
| 1739101 | 1722   | Bananas     | Null      | 24.72      | 10-02-2009 20:45:38 |

## Extracting Y

It can be the case where there is a dataset, where what you're trying to predict is not already a feature of the data. This does not always happen, but when it does, feature engineering is required to move forward in the modeling process.

You notice that you're not provided with the number of sales that month, so you are forced to extract that feature. This is a relatively easy task; you first create a column with all ones in it, then use a sum aggregation of the data by each month. This feature engineering will give you a new dataset.

## Extract for other features

Often the most useful features in the data are ones created from data you have. There are a variety of ways to create columns from numerical data. Common features involve different aggregations of the data.

Your company's data makes up a pretty bland dataset. It almost feels like there isn't much you can do with the data, but this is where feature engineering becomes useful. Since the data has a few different numerical columns, you could consider taking the aggregation of SaleID by the average ItemPrice.

## Perform feature engineering with datetime data

Timestamps allow for unique types of feature engineering that are extremely useful. This is because a dataset that is structured around time often operates differently than other datasets. The first technique is moving the average, which enables you to see the patterns over any length of time and improve model performance. (You can also use other moving aggregations.) The second technique is differencing, which enables you to find the differences in values over time.

In the example, the moving average could be extremely useful in the model. It may be helpful to look at the moving average TotalPrice on a month-to-month basis. This will help you identify a trend in the data.

## Summary

Feature engineering is an overlooked process that can strongly benefit the model if done correctly. If the data provided does not already have the graph's Y column, it's imperative to use feature engineering to extract it. Aside from that, much of vital data comes from feature extraction, especially in data formulated around dates.

------

## Next unit: Model training

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-science-in-azure/7-model-training)









# Model training

- 5 minutes

Model training is where you use the data to get a prediction. This process never looks the same because it's unique to the data available.

## Select the model

Many types of models are available, but not all of them are suitable for the outcome you want to predict. It's critical to identify whether you're trying to obtain a numerical or classification prediction. Then you can decide which type of model to use.

Because you're trying to predict the number of brooms that will sell each month, you pick an Autoregressive Integrated Moving Average (ARIMA) model. This is a modeling technique for time series analysis that helps with predictions concerning time.

## Split the data

![Screenshot of the steps to predictive modeling.](https://docs.microsoft.com/en-us/learn/data-ai-cert/intro-to-data-science-in-azure/media/7-steps-predictive-modeling.png)

When you train a model, you need to split your data into training and testing sets so that you don't train your model on all the data. You will need a way to test the performance of the model, which splitting the data into training and testing sets permits. The idea is to hold a subset of the data back and use it later to test the model's effectiveness.

After you feed the data to the model, be sure you don't give it the answer; make the model predict the answer.

Next, compare the predictions against the actual values to see how well the model performed. Data leakage, also known as *bias*, occurs when data included in the training set strongly correlates to what you're trying to predict. In other words, the training data includes information about what you're trying to predict. Predictions based on time requires you to use about 70 to 80 percent of the data for the training set, and 20 to 30 percent for the testing set. Otherwise, the train test split should be random.

When using time series data, it's essential to split the data based on time. Since our data goes from 2009 to 2014, we will use the data from 2009 to 2013 for the training set, and 2014 for the testing set.

## Cross-validate the data

When building a model, another common practice to improve model performance is cross-validation. This method splits the data into subsets of the full dataset to ensure you're not overfitting a model to one training set. *Overfitting* means that the model works well only with the data used to train it. This happens when too many data elements are used in model training. A sign of overtraining is when you get a high level of prediction accuracy, such as anything close to 100%. Cross-validation is often used in tandem with the train test split.

The data in our example is based on time, so we'll skip this step. This is because we only use cross-validation when the data used for prediction are the differences of the projections. This is often the case when a trend exists in the data.

## Obtain a probabilistic prediction

Everything we have done has led up to this point in the data science process. This is generally the glorified portion of what data scientists do. Obtaining a prediction can be simple once everything else is in place. Since you have chosen the ARIMA modeling technique, you simply call the ARIMA model and look at the results.

## Summary

This section is an overview of how to approach model training. By choosing the correct model, splitting your data into training and testing sets, and cross-validating your results, you'll improve your solution and avoid overfitting. In the next section, we'll discuss how to evaluate the model.

------

## Next unit: Model evaluation

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-science-in-azure/8-model-evaluation)









# Model evaluation

- 5 minutes

This part of the process uses the results from the model to see how well it did in predicting the outcome, referred to as *Y*. Depending on how well your model performs, you might need to fine-tune some hyper-parameters within the model to improve results.

## Tune the hyperparameters

*Hyperparameters* are parameters used in model training that cannot be learned by the training process. These parameters must be set before model training begins. Hyperparameters control how model training is done, which can have a significant impact on model accuracy. An example of a hyperparameter is the K parameter of the KNN model. This model defines regions of similar classes of items and determines which class a new item falls into by looking at the other items it has already classified. Basically, KNN asks "what is this new item most similar too?".

The K parameter tells the model how many other items to consider in making the determination. A K of 1 means only look at the single most similar item, and a K of 3 means look at the three most similar (closest) neighbors.

The value of K can have a significant impact on model accuracy. Deep learning models use several hyperparameters. However, when there is a large amount of data, tuning hyperparameters can be a computationally heavy task for a machine. If the dataset isn't too large, a process called *grid searching* allows you to get more accurate results as to which hyperparameters are best for your data because it looks at many more cases for each parameter. Another approach called the *random search method* searches randomly for the best hyperparameter values. This method is much less expensive computationally.

Since the dataset is only 10,000 rows, you move forward with grid searching. Note that when using this method, two hyperparameters need to be defined: learning rate, and number of layers help identify the extent of fine-tuning.

 Tip

Hyperparameter tuning should be used with cross-validation so that the model is not overfitted to the training dataset.

Models can be configured to improve accuracy using hyperparameter tuning. This enables you to improve probabilistic outcomes, but at the cost of increased compute resources and time.

Don't worry if you don't understand this if you're not a data scientist. The key takeaway is that models can be configured.

## Evaluate the results

This is the final step of the modeling process. However, since you'll usually have the modeling process repeat more than once, the first time this step runs is usually is not the end. When you evaluate the results you'll look at how accurate or inaccurate your predictions are. Let's look at two different techniques for evaluating results: you can evaluate a classifier model, or assess a numerical prediction model.

### Look for accuracy and precision

When evaluating a classification model a couple of metrics that are useful are accuracy and precision. To understand these terms, it's essential to understand what a confusion matrix is.

A confusion matrix includes the following:

- **True positive**: the number of times a model predicts true (or yes) when it is actually yes
- **True negative**: the number of times a model predicts false (or no) when it is actually false
- **False negative**: the number of times a model predicts false when it is actually true
- **False positive**: the number of times a model predicts true when it is actually false

This data is formatted in a matrix format to understand how accurate the predictive model is:

|                  |    Predicted No    | **Predicted Yes**  |
| :--------------- | :----------------: | :----------------: |
| Actually No      |   True Negative    | **True Positive**  |
| **Actually Yes** | **False Negative** | **False Positive** |

**Accuracy** is the value of accurate predictions of yes and no over the total number of predictions. You want this number to be as close to 1 as possible.

$${\dfrac{true\ positive + true\ negative}{true\ positive + true\ negative + false\ positive + false\ negative}}$$

You want the result to be as close to **one** as possible.

*Precision* is a measure of the consistency of the predictions. This is represented by the following equation.

$${\dfrac{true\ positive}{true\ positive + false\ positive}}$$

As with accuracy, the precision of your model increases as the result moves closer to **one**.

## Evaluate the metrics with mean squared error

Mean squared error (MSE) is one of the most popular model evaluation metrics in statistical modeling. It allows you to look at how far your predictions are on average from the correct values. In the example with time series analysis, MSE is a valid approach to model evaluation.

The few metrics we have examined are just a subset of what is available for model evaluation. The type of model will drive the direction of the model evaluation, but the technique you choose will depend on whether the model is a classification or numerical prediction.

------

## Next unit: Model deployment

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-science-in-azure/9-model-deployment)









# Model deployment

- 5 minutes

Model deployment is the final stage of the data science procedure. It is often done by a developer, and is usually not part of the data scientist role. Deployment typically means putting the resulting model into an environment where it can be called (or *consumed*) by applications.

There are many considerations for how you deploy a model. Model deployment can involve many things, but it always depends on how the business is looking to implement the model.

Using our example, the model deployment process could be as simple as choosing to implement the results of the model by stocking the shelves accordingly. It could also be as complex as building an application or integrating results into a website using HTML code.

------

## Next unit: Specialized roles in the Data Science process











# Specialized roles in the Data Science process

- 5 minutes

The data science process is often completed by a team of people with different roles, which are described in the following sections.

## Business analyst or domain expert

The business analyst or domain expert provide the deep business understanding to accurately guide the project. They understand the functional area and data. Some of the tools they use include but are not limited to Microsoft Excel, and query tools such as SQL.

## Data engineer

The data engineer prepares the data for use by the data scientist in model training. This step, known as *data wrangling*, cleans and transforms the data.

Common tools the data engineer will use include but are not limited to:

- SQL
- Extraction, transformation, and loading (ETL) tools
- Apache Hadoop
- MongoDB
- Apache Spark
- Python
- R

## Developer

The developer is responsible for model deployment, and potentially development of the application that will use the model to score new data. This means they build out the platform or the method for the model consumption and integration into the business, and possibly both.

Common tools the developer will use include but are not limited to:

- HTML
- CSS
- Python
- C#, Java, or JavaScript
- Source code control (Git, Svn)

## Data scientist

The data scientist is responsible for understanding the data, and training and testing the model. They will likely be involved with the other roles as they are at the heart of the process.

Common tools the data scientist will use include but are not limited to:

- Python and related packages
- R and related packages
- Apache Spark Databricks
- Microsoft Azure Databricks

------

## Next unit: Summary

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-science-in-azure/11-summary)









# Summary

- 5 minutes

In this module you learned that data science is a process of getting valuable information, and answering questions by analyzing the data with an emphasis on statistical methods, computing power, and automation. The idea of data science is to use historical data to predict something. To do this, you use data values that you know to predict something you don't know. This requires having historical data that has both the outcome you want to predict and other data that correlates to the outcome value.

You also learned that the types of questions that can be answered through data science vary greatly. Data science is based on probabilities so along with predicted outcomes, the estimated probability of the outcomes is a critical consideration.

You learned that when a business is looking to answer a data-driven question, they must follow a set of predefined steps, known as the *data science process*, and know what these steps involve. The process of data science includes more than one role.

Finally, you learned that the roles within this process are business analyst, data engineer, data scientist, and developer. Even though there can be some overlap, each of these roles are important and play a different part in the process.

## Check your knowledge

\1. 

Which of the following is not a specialized role in the Data Science Process?



Database Administrator



Data Scientist



Data Engineer

\2. 

Model feature engineering refers to which of the following?



Selecting the best model to use for the experiment.



Determine which data elements will help in making a prediction and preparing these columns to be used in model training.



Exploring the data to understand it better.

\3. 

The Model deployment involves.



Calling a model to score new data.



Training a model.



Copying a trained model and its code dependencies to an environment where it will be used to score new data.











# PART 2: Choose the Data Science service in Azure you need



# Introduction

- 5 minutes

Microsoft Azure offers many different products for machine learning and the data scientist. These products each have different purposes that help with various aspects of the data science process. The challenge is determining which product is best suited for each task.

 Note

This module assumes a knowledge of data science terms and processes. If you are new to data science, we recommend you go through the [Data Science for Beginners](https://docs.microsoft.com/azure/machine-learning/studio/data-science-for-beginners-the-5-questions-data-science-answers) video series.

## Learning objectives

In this module, you will:

- Differentiate each of the Azure machine learning products.
- Identify key features of each product.
- Describe the use cases for each service.

------

## Next unit: Machine Learning options on Azure

[Continue](https://docs.microsoft.com/en-us/learn/modules/choose-data-science-option-in-azure/2-ml-options-on-azure)







  

# Machine Learning options on Azure

- 5 minutes

Microsoft provides several Azure platforms that help with the machine learning process. All these products simplify the data science process in unique ways. They each have different features and purposes which we will explore here.

The following table summarizes some of these services.

| Product                              | What it is                                                   | What you can do with it                                      |
| :----------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| Azure Machine Learning service       | A managed cloud service for Machine Learning.                | Train, deploy, and manage models in Azure using Python, Azure CLI, and Azure portal. |
| Azure Machine Learning Studio        | A drag-and-drop visual interface for Machine Learning.       | Build, experiment, and deploy models using preconfigured algorithms. Ideal for learning about Machine Learning. |
| Azure Databricks                     | Apache Spark–based analytics platform with an integrated notebook interface that seamlessly integrates with Azure Active Directory (Azure AD) and data services. | Build and deploy models and data workflows with big data.    |
| Azure Data Science Virtual Machine.  | A virtual machine with preinstalled data science tools.      | Develop machine learning solutions in a preconfigured data science environment. |
| SQL Server Machine Learning Services | Integrated with Microsoft SQL Server, this scalable analytics server supports the Python and R language. | Build and develop models in an on-premises SQL server that scales to match the SQL Server engine. Microsoft Machine Learning Server is also available as a cluster type in Azure HDInsight. |

Let's explore these services in more detail.

## Scale, automate, and deploy with Azure Machine Learning service

The Azure Machine Learning service supports data science pipeline integration with Azure. It allows you to scale up and automate:

- Model management
- Model training
- Model selection
- Hyper-parameter tuning
- Feature selection
- Model evaluation

The Azure Machine Learning service also enables you to more easily deploy your trained models to Azure containers where you can use them. The key advantage of this service is that it makes it easier for your data science project to utilize containerization and automation, resulting in better results in less time.

Examples of tools you typically use with this service include:

- Azure Machine Learning SDK
- Python
- Jupyter Notebook
- Microsoft Visual Studio
- JetBrains PyCharm
- Your favorite IDE

### Utilize the Azure Machine Learning Studio platform

Azure Machine Learning Studio is a GUI-based platform that's an excellent place for beginner data scientists and analysts to learn. As an interactive platform, it provides a visual display for the modeling process, including deployment options. Azure Machine Learning Studio integrates a drag-and-drop method of the iterative data science process for simple use. It also includes an automated deployment service that supports REST API calls to score data.

Examples of tools included with Azure Machine Learning Studio are:

- Data visualization
- Drag-and-drop interface
- Azure (Jupyter) Notebooks
- Project samples

 Tip

Azure Machine Learning Studio is primarily a learning platform and for limited-scale use.

### Azure Databricks platform

*Azure Databricks* is a secure, all-in-one data science team collaboration platform. It includes a powerful notebook interface, job scheduling, Azure Active Directory integration, granular security control, and seamless Azure integration. Azure Databricks has a GUI-based cloud portal that makes it even easier to use the Spark big data platform. You can more easily create and modify Spark clusters, and turn them off when not using them without losing data.

Azure Databricks features include, but are not limited to:

- Azure Databricks notebooks, which support SQL, Python, R, Scala, and Java
- Job scheduler
- Local built-in Blob Storage
- Seamless, secure access to Azure data services such as Azure Blob Storage, Azure SQL database, Azure SQL Datawarehouse, and Azure CosmosDB
- Graphical UI to quickly spin up and scale Spark clusters
- Proprietary Spark optimizations

### Azure Data Science Virtual Machine

Built specifically for data science, *Azure Data Science Virtual Machines* (DSVMs) are preconfigured virtual machines you create in Azure that have many popular machine learning tools preinstalled. It provides data scientists a simple way to begin and iterate through the modeling process.

Examples of DSVMs tools include:

- SQL Server / Machine Learning Server
- Microsoft R Open
- Jupyter notebooks
- Anaconda Python
- Sample code demonstrating how to use various Azure-based Machine Learning services

### SQL Server Machine Learning Services

*SQL Server Machine Learning Services* runs on the SQL Server on-premises platform, and supports scale up and high performance of Python and R code. With it, you can work with SQL Server data in place. You also get all the SQL Server features including tighter security, excellent performance, the ability to schedule model training with the SQL Agent service, and persistence of models to database tables. In addition, you can encapsulate Python and R code in stored procedures, and they can interoperate with T-SQL so you can have the high performance of T-SQL with the advanced Machine Learning features or R and Python.

Along with core Python and R tools, SQL Server Machine Learning Service includes a set of components for data scientists.

- Python components and packages for data manipulation, transformation, visualization, and analysis.
- R packages such as RevoScaleR, MicrosoftML (R), opalR, and sqlRUtils to perform data science tasks in the R language.

------

## Next unit: Data Science Virtual Machine

[Continue](https://docs.microsoft.com/en-us/learn/modules/choose-data-science-option-in-azure/3-dsvm)










# Data Science Virtual Machine

- 5 minutes

The Data Science Virtual Machine (DSVM) platform is designed to provide a virtual machine in which you can complete everything within the data science process.

## What is Data Science Virtual Machine (DSVM)?

*Azure DSVM* is a customized virtual machine on Azure Cloud Services, with many popular data science tools preinstalled and preconfigured for building data science applications. These tools are designed to help business analysts, data engineers, data scientists, and developers.

![Screenshot of a Data Science VM](https://docs.microsoft.com/en-us/learn/data-ai-cert/choose-data-science-option-in-azure/media/3-dsvm.png)

If you are a data scientist looking to maximize your environment with numerous preinstalled data science tools, DSVM is a good option.

## How to use DSVM

DSVM provides a jumpstart for machine learning model training. To use a Windows-based DSVM, you can use Microsoft Remote Desktop to access it using the administrator credentials defined when the DSVM was created. You can learn more about how to build a model in a DSVM by accessing the tutorials available on the virtual machine.

For Linux-based DSVMs, you connect to it using of the following methods:

1. SSH for terminal sessions
2. X2Go for graphical sessions
3. JupyterHub and JupyterLab for Jupyter notebooks

## Explore types of DSVMs

There are a various types of DSVMs that are available for different machine learning purposes.

### Supported operating systems

DSVM supports both Windows and Linux operating systems, with each offering various machine mearning tools. The key difference between the two servers is that Windows operating systems offer scalability with Machine Learning in SQL Server, and Linux does not.

### Deep Learning Virtual Machine

A *Deep Learning Virtual Machine* (DLVM) is a version of DSVM that offers a variety of deep-learning tools for building artificial neural networks—an algorithmic process that simulates the decision process of the human neural network.

### Geo AI DSVM

This version of a DSVM includes tools specific to Machine Learning that relate to geospatial data. Geo AI DSVM comes with other standard machine learning software, but it also includes ArcGIS, which is a commercial platform for Geo AI.

------

## Next unit: Azure Machine Learning Studio

[Continue](https://docs.microsoft.com/en-us/learn/modules/choose-data-science-option-in-azure/4-azure-ml-studio)








# Azure Machine Learning Studio

- 5 minutes

**Microsoft Azure Machine Learning Studio** is a web-based drag-and-drop learning platform you can use to build, test, and deploy machine learning models without writing any code. It provides a visual display of datasets and models with a drag-and-drop interface and includes many tools, such as Azure Notebooks to process data and visualize output. The interactive visual workspace allows data scientists of all skill levels to use the platform to easily create and iterate predictive analysis models.

Azure Machine Learning Studio allows you to bring in data, cleanse and transform the data, train and score a model with the option of deploying it on the web. If you are beginning your journey to learning data science, this platform is an intuitive way to help you understand the data science process.

![Screenshot showing the Azure Machine Learning Studio site](https://docs.microsoft.com/en-us/learn/data-ai-cert/choose-data-science-option-in-azure/media/4-azure-ml-studio.png)

## Use Azure Machine Learning Studio

Azure Machine Learning Studio provides several sample datasets and experiment models such as the **Prediction of studio performance** experiment which uses a regression model. These different samples demonstrate various ways to train models and process data. For example, here's a screenshot of an experiment showing how to implement a restaurant recommender system.

![Screenshot of the Azure Data Science portal with a sample experiment loaded](https://docs.microsoft.com/en-us/learn/data-ai-cert/choose-data-science-option-in-azure/media/4-azure-ds-portal.png)

You can then import your own data and process it with the built-in machine learning models. There's no programming required - just connect your datasets visually to the prebuilt modules to construct your analysis models. As you modify the various functions and their parameters, your results converge until you have a trained, effective model. Then you can then publish the model as a web service so others can access it.

Here's a visual overview of the workflow used with Azure Machine Learning Studio showing how the data is turned into trained models.

![Diagram showing the capabilities of Azure ML Studio](https://docs.microsoft.com/en-us/learn/data-ai-cert/choose-data-science-option-in-azure/media/4-azure-ml-framework.png)

While programming experience is not required, you can customize the logic using scripts written in Python or R - this allows you to write custom algorithms and intermix them with the standard modules provided by the platform.

You can learn more by signing into the [Azure Machine Learning Studio](https://studio.azureml.net/) and going through tour.

------

## Next unit: SQL Server / Machine Learning Server

[Continue](https://docs.microsoft.com/en-us/learn/modules/choose-data-science-option-in-azure/5-sql-ml-server)









# SQL Server / Machine Learning Server

- 5 minutes

**SQL Server Machine Learning Services** is an add-on for SQL Server that allows you to execute Python and R code on SQL Server. This platform enables you to integrate data science processes using Python or R within the local SQL Server environment, which eliminates the need to switch between the database and machine learning environments. You get all the features of SQL Server with scalable machine learning.

![Screenshot of both the Machine Learning and SQL Server.](https://docs.microsoft.com/en-us/learn/data-ai-cert/choose-data-science-option-in-azure/media/5-ml-server-sql-server.png)

 Note

Machine Learning Services (with R) is currently in public preview for Azure SQL Database.

There are several advantages to using the SQL Server Machine Learning Services to perform data science tasks.

- **Security**. Because the data processing occurs closer to the source of the data, it avoids the movement of the data which limits the exposure.
- **Performance**. Along with data locality, SQL Server is optimized for set-based operations and includes support for in-memory tables which provides better throughput for many data science operations.
- **Consistency**. SQL Server is often the hub for data management tasks and applications in an organization. By using data that resides in the database or reporting warehouse, you ensure that the data used by machine learning solutions is consistent and up-to-date.
- **Efficiency**. You can use other tightly integrated tools such as PowerBI and Azure Data Factory to report and analyze results.

------

## Next unit: Spark on HDInsight

[Continue](https://docs.microsoft.com/en-us/learn/modules/choose-data-science-option-in-azure/6-sqark-on-hdinsight)









# Spark on HDInsight

- 5 minutes

**Azure HDInsight** is an Azure platform as a service (PaaS) Apache Hadoop offering. It is based on the Hortonworks distribution of Hadoop. When you provision an HDInsight cluster, you specify which type of a Hadoop platform you want.

HDInsight provides several benefits.

- You can quickly spin up big data clusters on demand, scale them up or down based on your usage needs, and pay only for what you use.
- Extract, transform, and load your big data clusters on demand with Hadoop MapReduce and Apache Spark.
- Meet industry and government compliance standards and protect your enterprise data assets using an Azure Virtual Network, encryption, and integration with Azure Active Directory.
- Integrate seamlessly with other Azure services, including Data Factory and Data Lake Storage, for building comprehensive analytics pipelines.
- Use your preferred productivity tools, including Visual Studio, Eclipse, IntelliJ, Jupyter, and Zeppelin.
- Write code in familiar languages such as Scala, Python, R, JavaScript, and .NET.

For scalable machine learning, we are only concerned with the HDInsight Spark implementation.

## What is Spark?

Apache Spark is an open-source big-data platform that uses a *scale-out* approach. This is where multiple machines working together to process data. Unlike Hadoop, Spark works in-memory as much as possible. This results in much faster processing than Hadoop.

**HDInsight Spark** is an implementation of Apache Spark on Azure HDInsight. It supports massive scale for data querying, wrangling, and machine learning model training. A cluster has a master server that controls the other servers in the cluster. By splitting the work among multiple machines, performance is greatly enhanced. It shares the data source across all the servers by storing the data into Azure Blob Storage.

 Tip

Data scientists who are comfortable working with the native Spark interface and want complete custom control of the data science process should consider using HDInsight Spark. For the data science team looking for an all-inclusive, user friendly, secure, collaborative, Spark-based environment, Azure Databricks may be a better solution.

HDInsight Spark has a version that uses R Server as a processing front end. The R Server proprietary model training libraries scale out machine learning over the Spark cluster for big data model training. HDInsight integrates with other Azure Services as shown in the following diagram.

![Screenshot of the Spark framework.](https://docs.microsoft.com/en-us/learn/data-ai-cert/choose-data-science-option-in-azure/media/6-spark-framework.png)

------

## Next unit: Azure Databricks

[Continue](https://docs.microsoft.com/en-us/learn/modules/choose-data-science-option-in-azure/7-azure-databricks)







# Azure Databricks

- 5 minutes

**Azure Databricks** is a secure, all-in-one collaboration platform for data science teams. It includes a powerful notebooks interface, job scheduling, Active Directory integration, granular security control, and seamless Azure integration. It instantly provides data science teams with everything they need to create end-to-end machine learning pipelines for big data.

![Diagram showing the features of Azure Databricks](https://docs.microsoft.com/en-us/learn/data-ai-cert/choose-data-science-option-in-azure/media/7-azure-databricks.png)

## How Azure Databricks works

To use Azure Databricks, you provision an Azure Databricks Workspace using the Azure portal. The workspace provides all the assets you need. From there, you can add users that you want to have access to the workspace, and refine the level of access from with Azure Databricks. Here's a screenshot of the Azure Databricks landing page.

![Screenshot of the Azure Databricks landing page](https://docs.microsoft.com/en-us/learn/data-ai-cert/choose-data-science-option-in-azure/media/7-databrick-landing-page.png)

### Provided tools

The tools provided include a powerful notebook service that supports big data queries and visualizations. Notebooks can include all Spark-supported languages (including Scala, Java, SQL, Python, and R) in the same notebook. This enables you to use your language of preference, but switch to another language if you need to.

An advanced job scheduler allows you to schedule notebooks to run whenever you want. If the cluster isn't running, the job scheduler will create it automatically and delete it at the end of the job.

Assets such as notebooks can be shared and worked on collaboratively. Best of all, you don't need to worry about the complexities of configuring Spark clusters. The Azure Databricks GUI provides an easy-to-use interface to create and edit your cluster, and even set automatic turn-off for clusters after a period of disuse. You can delete clusters without losing any data or notebooks, so there's no need to keep clusters running if you don't need them.

In addition, Azure Databricks has several other features and tools including:

- Granular security configuration
- PySpark and SparkR
- Command-Line interface to perform tasks

------

## Next unit: Azure Machine Learning Service

[Continue](https://docs.microsoft.com/en-us/learn/modules/choose-data-science-option-in-azure/8-azure-ml-service)







# Azure Machine Learning Service

- 5 minutes

**Azure Machine Learning service** provides SDKs and cloud services you can use to integrate your data science pipelines with Azure. It allows you to scale up and automate:

- Model management
- Model training
- Model selection
- Hyper-parameter tuning
- Feature selection
- Model evaluation

When you are ready, the service allows you to easily deploy your trained models to Azure containers where they can be used. The key advantage of Azure Machine Learning service is that it makes it easier for your data science project to utilize containerization and automation, meaning you get better results in less time.

## What is included in Azure Machine Learning service

The Azure Machine Learning service supports open-source technologies, which include a plethora of packages for practicing machine learning via Python. Azure Machine Learning service includes common data science tools as extensions. If you're wondering why this would be beneficial for a data scientist, this technology permits the use of at-scale data because it can run on a local machine, then be scaled up to the cloud when needed.

![Screenshot of the Azure Machine Learning framework.](https://docs.microsoft.com/en-us/learn/data-ai-cert/choose-data-science-option-in-azure/media/8-aml-framework.png)

## Roles in Azure Machine Learning service

The platform is designed to support three specific roles:

1. Data Engineer
2. Data Scientist
3. Developer

### Data Engineer

The primary task a data engineer will do with Azure Machine Learning service is to ingest and prepare data for analysis. You can prepare your data locally, or leverage Azure containers. To prepare/transform the data you can use the open-source Azure Machine Learning Data Prep SDK, or the Pandas open-source library.

### Data Scientist

The Azure Machine Learning service doesn't replace any of your data science analysis tools.

You can bring all of your existing machine learning pipelines into Azure Machine Learning service and incorporate your Python code to utilize the powerful Azure Machine Learning service features. In addition to support for deep learning, many model training frameworks are supported, including:

- Scikit-learn
- TensorFlow
- PyTorch
- Microsoft Cognitive Toolkit (CNTK)
- Apache MXNet

![Screenshot of multiple Icons.](https://docs.microsoft.com/en-us/learn/data-ai-cert/choose-data-science-option-in-azure/media/8-combined-icons.png)

### Developer

Once a model has been built and trained, you can create an *image* of the model and all components needed to use the model. An image contains:

1. The model.
2. A scoring script or application which passes input to the model and returns the output of the model.
3. The required dependencies (for example, the Python scripts or packages needed by the model or scoring script).

Images can be packaged either as Docker images, or field programmable gate array (FPGA) images.

Azure Machine Learning service can deploy images to either a web service (running in Azure Container Instance, FPGA, or Azure Kubernetes Services), or an IoT module (using IoT Edge). Once deployed, developers can invoke models from their applications to process data and return results.

------

## Next unit: Summary

[Continue](https://docs.microsoft.com/en-us/learn/modules/choose-data-science-option-in-azure/9-summary)






# Summary

- 5 minutes

In this module, we discussed each of the products available for Machine Learning on Azure. The key takeaway is to understand how to differentiate each of them, because you can utilize every product in different ways.

Although many of these products provide similar tools, their functionalities vary. For example, some of them are meant to be learning tools, while others are more for professional use. Our hope is that now you can identify which tools are best for your needs, and what the tools can do for you in your Machine Learning practice. In the following module, we briefly discuss what has been covered in this course to verify your understanding of the topics explained.

## Check your knowledge

\1. 

Azure Machine Learning service supports which programming language.



R



Julia



Python

\2. 

Azure Databricks is built on which Big Data platform?



Azure SQL Data Warehouse



SQL Server



Apache Spark

\3. 

Which is not an operating system available for an Azure Data Science Virtual Machine?



Windows



Linux



Apple iOS