# Data_Science_inProduction
The main purpose of this repository is to show the evolution of my Data Science in Production brazilian course.

![Image description](https://github.com/panambY/Data_Science_inProduction/blob/master/data_science_em_producao_logo.png)

This repositore has the main purpose to show the evolution of my Data Science in Production brazilian course.
I will show the codes, the abstract about my learnings and the post which I writing about this course content.

# Index<br>
## 1.0 - About the course <br>
## 2.0 - Content of the course <br>
## 3.0 - Codes of the evolution <br>
## 4.0 - Conclusion <br>

![Image description](https://github.com/panambY/Data_Science_inProduction/blob/master/gif_minions.gif)

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

# 3.0 - Codes of the evolution <br>

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


