# Rossmann Store Sale

## Data_Science_inProduction

The main purpose of this repository is to show the evolution of my Data Science in Production brazilian course.

![Image description](https://github.com/panambY/Data_Science_inProduction/blob/master/image/data_science_em_producao_logo.png)

This repositore has the main purpose to show the evolution of my Data Science in Production brazilian course.
I will show the codes, the abstract about my learnings and the post which I writing about this course content.

# Index<br>
## 1.0 - About the course <br>
## 2.0 - Content of the course <br>
## 3.0 - Explanations <br>
## 4.0 - Conclusion <br>

![Image description](https://github.com/panambY/Data_Science_inProduction/blob/master/image/gif_minions.gif)

# 1.0 - About the course <br>

This data science course is not a traditional course easily found on the market. His focus is not on teaching the tools used by a data scientist, such as: Python, Pandas, Numpy, Sckit-Learn, Machine Learning, SQL, among others. However, he also does not require you to be an expert on the subject, but you must have at least a sense of the topic and the tools.

Its focus is on the execution of Data Science projects. For that reason there could not be a better title for it: Data Science in Production.

It is a course that aims to prepare the data scientist for the market, learning what companies expect when looking for a professional qualified to solve their problem.

All the knowledge necessary for you to perform the tasks within the course he teaches as you pass the contents.

I've been in the market for a while working and getting to know or taking some courses. I can assure you that a course with this type of material is rare and worth a lot for your data scientist career.

# 2.0 - Content of the course <br>

Module 01 - Understanding the Business Problem

Module 02 - The Data Description

Module 03 - Feature Engineering

Module 04 - Exploratory Data Analysis

Module 05 - Data Preparation

Module 06 - Feature Selection

Module 07 - Machine Learning Models

Module 08 - Hyperparameter Fine Tuning

Module 09 - Error Interpretation and Translation

Module 10 - Deploying the Model In Production

Module 11 - Creating the Bot in Telegram

Bonus 01 - Python and Git for Data Scientist

Bonus 02 - Results Storytelling

Bonus 03 - Study Map for Data Science

Bonus 04 - Data Science Office Hour

# 3.0 - Explanations <br>

## Module 01 - Understanding the Business Problem <br>

In this module he starts by talking about the 4 Topics to understand business problems. <br>
As a background, the first and main teaching he says is "Don't go immediately to start the project that you were told to do".<br>
- Understand what is the motivation behind that request, the context. Go to whoever asked you to and try to find out where this demand came from and within what situation. <br>
- Understand the root cause of the problem. What the company really wants with the result of this project. What problem are they trying to solve with him?<br>
- Find out who owns the problem, the Stakeholder. Whoever started the order will usually be someone big in the company. Who is the "owner" of the section within the company that will be affected by the outcome of the project. That person will certainly be able to better explain the purpose of it all. <br>
- After defining and maintaining or not the main purpose of the project, define the format of the solution. What format of the solution will you deliver. In this process, granularity, type of problem, potential methods and delivery format will have to be defined.

granularity: per day, per week, monthly, per store, per product, per category, per area; <br>
type of problem: regression, classification, prediction, clustering; <br>
potential methods: neural network, time series; and <br>
delivery format: dashboard, csv, image in email attachment, on the cell phone.

To start learning the entire process within a Data Science project, data from a Kaggle competition that belongs to ROSSMANN and will be called ROSSMANN STORE SALES will be used. <br>
To need it just click on this link:https://www.kaggle.com/c/rossmann-store-sales

Within this competition the answers to understand the business problem will be as follows:<br>
- Motivation -> CFO requested this solution during a monthly results meeting<br>
- Root Cause of the Problem -> Investment in Store Renovation<br>
- Who is the Stakeholder -> The CFO<br>
- Solution Format -> granularity (daily sales in $ for the next 6 weeks), type of problem (prediction), methods (time series, regression and neural networks) and delivery format (via cell phone)

At the end of this Module, the project management method called CRISP-DS was taught. It is better known as CRISP-DM, but as we are applying here for Data Science we will use DS instead of DM. Its main characteristic is that it is a CYCLICAL method of development, where you will assume that you will go through the same stage several times. This is important for several reasons, such as:<br>
- You will already have a 1st end-to-end version of the project<br>
- Speed in delivering value <br>
- Mapping all possible problems<br>
- Assists in the common mistake of being "in love" with a specific stage and not worrying about the whole

Its steps are as follows: <br>
- Business Question <br>
- Understanding the Business <br>
- Data Collection <br>
- Data cleaning <br>
- Data Exploration <br>
- Data Modeling <br>
- Machine Learning Algorithms <br>
- Evaluation of Algorithms <br>
- Production Model <br>

It is worth mentioning that the concern in the first cycle is not with the accuracy of the model, but with finishing the first cycle. Because then we will be able to identify if there is a problem when we implement the solution. <br>
If a problem is found in the implementation, the possible solutions would be: Give up the project, seek from the engineering team to change the data supply so that you have the necessary data or assume the low accuracy of your model with the absence of the data.<br>
Finally, when the first cycle ends, it is restarted at the Business Understanding stage.

## Module 02 - The Data Description <br>

When cleaning data, the first thing to do is a descriptive analysis and then apply the cleaning itself. This procedure is important because it allows us to see the size of the problem that we will be dealing with and how challenging it will be. In addition, it will also help you in the process of stipulating the project's execution time. <br>
There is 4 main points within the descriptive analysis and that will help you do an appropriate cleaning so that your model does not have difficulties in generating a good accuracy:

- Amount of data -> do I have the necessary tool to work with this amount of data? Do I have the right resources to perform this task?<br>
- Variable types -> what methods will be needed to be executed throughout the project for transformation, encoding, correction or generation of new variables? <br>
- Amount of missing data -> will I be able to continue with my project in face of this amount of NaN? What is the reason for missing data? <br>
- Summary of data -> Here the goal is for you to get a general sense of the size of your data. Various techniques of Descriptive Statistics will be used so that you can have access to this knowledge.

Obs: When you are dealing with the missing value there are three ways which you can solve this problem: <br>
- give up of the project because there are several missing values <br>
- fill the empty spaces with algorithms <br>
- understand the model business and try to fill the missing values

Inside the part of Descriptive Statistics, there are two advantages about using this method: <br>
- Knowing a better understand about the business <br>
- To detect some error

These purposes we can achive by apllying two in Basic Statistics thecniques , which are: <br>
- Central Tendency-> mean, median, mode <br>
- Dispersion -> standard deviantion, variance, minimum, maximum, range, skew, kurtosis

Obs: For numerical variables use statistical code in in python, but for categorical variables use box plot graph.

## Module 03 - Feature Engineering <br>

For Data Exploration to be well done, it is necessary to follow 3 (three) processes that will guide you efficiently so that the data can be well prepared until the last process, which is exploratory analysis.

- List of Hypotheses -> Through the Mind Map tool you create a Hypothesis Map that then generates a Hypothesis List. This map has elements that will guide the creation of your list, which are: phenomenon, agents and attributes. Your project has the root problem or phenomenon to be solved. Present in this phenomenon are the agents that influence it. Each agent has characteristics or attributes. <br>
- Creation or derivation of variables -> With this List of Hypotheses you will prioritize your items following a business limitation, that is, if the data you will need to be used in the exploratory phase you already have it available in the dataset or you will have to do some data engineering to obtain it over there. The rule is very simple: if you already have the data available, the assumption will be maintained, if not, it will be removed and can be used in the next cycles if your model does not perform well. <br>
- Filtering variables -> First of all it is important to differentiate between filtering and selection of variables. The first has to do with restrictions according to the business where it is inserted and the second with the relevance that it has for the model. It is very common, if not almost mandatory, that your dataset has data that has been collected in different parts during your company's business process, that is, it has data that was acquired at the beginning of the mat and data that is acquired almost at the end her. To prevent this from happening, you will do the filtering of the variables before the Exploratory Data Analysis (EDA) so that in the next phase you have not only all the variables necessary to validate the assumptions in the Hypothesis List, but also those that will actually be available for use in the model.

## Module 04 - Exploratory Data Analysis <br>

When we do EAD we have to find out how the variables impact the phenomenon we are trying to predict and the strength of that impact on the response variable. This helps us to know the reason that your Machine Learning model may not have performed well at the end of your project. Without EDA you would try to solve this problem by going through a manual trial and error process, which is very time consuming and ineffective.

Objectives: <br>
- Gain business experience; <br>
- Validate Business Assumptions (insights); <br>
- Realize variables that are important to the model.

The types of analysis: <br>
- Univariate Analysis; <br>
- Bivariate Analysis; <br>
- Multivariate Analysis.

## Module 05 - Data Preparation <br>

Within Data Modeling, we have Data Preparation and they help us to model data for the training of Machine Learning Algorithms. This concern is motivated by the fact that most algorithms and ML are facilitated with numerical data and on the same scale.

- Normalization -> Rescala the center to 0 (zero) with standard deviation equal to 1 (one) and is used for variables with normal distribution. <br>
- Rescaling -> Its operation is similar to normalization, but there are some fundamental differences. The first would be that it reshapes between 0 (zero) and 1 (one) and no longer between +1 and -1. The second, and the most important difference, is that it will be used in variables with non-Gaussian distribution. <br>
- Transformation -> This method works in two different ways. The first one would be applying the encoding which would be the conversion of numeric data into categorical data. The second would be in relation to the transformation of nature, for example, we have the variable months that have the same sets of months that are from 1 to 12, that is, we can observe that they have a cyclical nature since after 12 it goes back to the 1 and so on. With that we can use a method that applies a transformation so that the algorithm can understand this cyclical nature.

## Module 06 - Feature Selection <br>

Always give preference to simpler models. These simpler models learn from simpler data sets. To arrive at this type of model we have to go through the process of removing collinear variables. When two or more variables explain the same part of the phenomenon they are called collinear and one of them can be removed.

The 3 Types of Selection of Variables: <br>
- Filter Method -> It takes into account relevance, which means how each variable explains a portion of the phenomenon. The Correlation Coefficient is the statistical way to discover this relevance, that is, it explains a little this relationship of intensity between the variables. <br>
- Embedded Method -> Unlike the Filter Method, which uses correlation as a criterion, here importance is used as a criterion. It is also known as the Embedded Method, as it is already embedded within several Machine Learning algorithms, that is, it is a by-product of learning these algorithms. <br>
- Wrapper Method -> This method is totally different from the previous ones and consists of adding the variables one by one and calculating their performance. If it goes up, the variable included last is relevant, but if the performance falls or is the same, the variable added last is irrelevant for the model.

## Module 07 - Machine Learning Models <br>

Learning the behavior of something with available variables and then generalizing it for the future.

- Supervisioned: <br>
a) classification -> used for variable categorical responses <br>
b) Regression -> used for variable numerical responses <br>
c) Time Series -> used to predict future behavior based on past behavior

- Unsupervised: <br>
a) Grouping or Clustering

- Semi Supervised: uses the concepts of Agent, Action, Environment and Reward <br>
a) Reinforcement Learning

## Module 08 - Hyperparameter Fine Tuning <br>

- Random Search: Randomly chooses the parameter values. <br>
a) Advantage -> Fast and low cost. <br>
b) Disadvantage -> You will hardly be able to choose the best combination of values.

- Grid Search: Choose all possible combinations between the parameter values. <br>
a) Advantage -> Defines the true values that maximize the learning of the model. <br>
b) Disadvantage -> Extremely time consuming and costly.

- Bayesiana Search: Uses Bayes' theorem to define parameter values. <br>
a) Advantage -> Faster than Grid Search and slower than Random Search. <br>
b) Disadvantage -> A little hard the understanding.

## Module 09 - Error Interpretation and Translation <br>

The importance of understanding the model's performance is being able to know how much value your model will bring to your company.

- Error Interpretation: <br>
a) MAE -> Mean Absolute Error. <br>
b) MAPE -> Mean Absolute Percentage Error. Shows the percentage of error for your model. <br>
c) RMSE -> Root Mean Squared Error. <br>
d) MPE -> Mean Percentage Error. Indicates whether your model is overfitting (negative value) or underfitting (positive value).

- Error Translation: <br>
a) Status Quo -> You measure the impact of your model in relation to the metric used by your company showing what it brought in value and what your model will bring. The goal is for your model to bring more value than the forecast metric currently used. <br>
b) Business Performance -> How much increment will your model add, that is, how much revenue will your model bring to the company.

## Module 10 - Deploying the Model In Production <br>

In this part, some Python code is built to assemble the entire structure that will trigger the classes and functions to make the model trigger when the store number is entered. In this first moment, the model will be stored in the cloud inside the Heroku platform and accessed through the Jupyter Notebook as a test to verify its correct functioning. <br>
The goal here is to make the prediction model accessible to anyone. To achieve this, an API is created.

The architecture of the model in production: <br>
- Handler API -> is the part that receives the requests and plays for the other parts so that the data is processed and then brings everything together, returning the final answer. <br>
- Data Preparation -> all the treatments and modifications we made to the data will be kept inside. When the Handler receives the raw data it will throw it here within this list of treatment codes so that they are prepared so that they can be ready to be used within the Machine Learning model. <br>
- Model Training -> this is our trained model that has been saved and will be placed inside this folder in our production architecture. The Handler will take the data processed within Data Preparation and play it inside the model so that it provides the prediction.

At the end of the construction of all this architecture and being put into production, the way it will be visualized can be through an App, Dashboard or a website.
