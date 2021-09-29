# CS3244 Project Proposal
CS3244 Group Project on Stock Market Data

### 1. Project Group Number
39

### 2. List of student IDs in your group
A0200877A, A0200864L, A0200882L, A0200498E, A0201185R

### 3. Dataset choice
**Which dataset from the curated list did you choose? If you plan to use more than one, select the primary one. If you selected a different dataset, use the open option and list it down, and you'll need to discuss it with our instruction staff.
It's highly encouraged that you select one of the curated datasets as your primary project data source.
Details of the curated datasets are on the CS3244 Project Datasets document: http://www.comp.nus.edu.sg/~cs3244/AY2122S1/datasets.html**

- Stock Market Dataset
https://www.kaggle.com/jacksoncrow/stock-market-dataset

### 4. Dataset description
**Write in your own words (1-2 sentences) what this dataset describes.**
**Rubric:
a) Does your description specify features and instances?
b) Do you describe the source and reliability of the data?**

- The dataset contains historical stock market price actions for NASDAQ listed companies. Each instance in the dataset represents the price actions(i.e. Open, Close, High, Low) and trade volume for a particular date.
 Features:
  - Date - Date of the trading day
  - Open - price at which the stock began trading
  - High - maximum price in the given date
  - Low - minimum price in the given date
  - Close - price at which the stock ended trading
  - Volume - total amount of trading activity
  - OpenInt - open interest, total number of outstanding derivative contracts, or future contracts held by market participants at the end of the trading day
  
 - **The prices(High, Low &Close) have been adjusted for dividends and splits.**

- The dataset is provided by a user on kaggle, Boris Marjanovic. The stock price data is open to the public. The data are reliable as constant feedback has been given by different users in the discussion section in the case where they found any errors in the data.


### 5. Project Title
- Title: Stock Market Prediction
- Description: Predict the close prices of a stock for a future time range to help traders in decision making, whether the trader should buy or sell the stocks.

### 6. Motivation
**Explain why this project is interesting and important.**

**Rubric:
Does your motivation clearly describe a problem? 
Does it justify the problem’s significance? What are the benefits of addressing this problem? Who benefits from solving it?**
- With the increasing stock data available and more companies being listed in the financial markets, it’s inefficient and merely impossible for traders to manually analyse and predict all the market trends. Hence, using machine learning to automate the stock market prediction process would be an efficient method to solve this problem.
- With a successful model, we are able to capture trade signals that would not be easily spotted by traders, hence more accurate predictions can be made to aid in decision making by the traders.



### 7. Statement of the Problem/Task
**A statement of the problem, issue, or task that you’re interested in studying. In particular, try to formulate the key questions (2 to 4 questions is probably a good number) that your group will answer in the project.
As this proposal document is self-contained, you should restate your project topic and domain.
The information you provide here will also help to assign appropriate reviewers.**

**Rubric:
a) Does the proposal outline a problem statement, issue, or task that the group is interested in studying?
b) Does it formulate a few (2 to 4) questions that the group proposes to address?**
- Title: Stock Market Prediction
- Domain: Time Series Analysis
- Description: Predict the close price of a stock for future time range to help traders in decision making, whether the trader should buy or sell the stocks.

- What kind of data transformations (e.g. technical analysis) are needed for our dataset, how many features should be selected as the explanatory variables for our time series model?
- Which models are suitable for this context?
- How far ahead of the time can our model predict with acceptable accuracy?
- How do we evaluate our model?

### 8. General Approach
**A high-level description of the general approach you’ll use to address the questions. Survey on the current progress on the problem/task. Sketch out what evidence you are planning to gather (e.g., how you can answer the questions through experiments on the data).**

**Rubric:
a) Does the proposal contain a high-level draft description of the general approach proposed to address the questions?
b) Does it include preliminary plans for evaluation, data gathering? I.e., how the team plans to answer the questions through experiments on data.**

- We will test out different models such as Linear Regression, k-Nearest Neighbors, Auto ARIMA, etc. and compare their performances, to evaluate which model gives the best performance. In addition, we will research more on the possible evaluation methods for our model prediction. We will explore different indicators in technical analysis to determine whether it is suitable to be used as one of the approaches for deciding on the features for our model.

 
### 9. Evaluation
**Include how you will evaluate your project. Propose what your team thinks is a satisfactory project outcome (C grade) and an excellent project outcome (A grade).**

**Rubric:
a) Does the proposal contain a high-level draft description of the general approach proposed to address the questions?
b) Does it include preliminary plans for evaluation, data gathering? I.e., how the team plans to answer the questions through experiments on data.**

- We will decide the levels of threshold for the error and correctness of our model (metrics to be decided) to evaluate our project outcome.
- Satisfactory outcome: Our model is able to predict a general trend on a bigger scale.
- Excellent outcome: Our model is able to follow closely to the actual trend with acceptable fluctuations.
- Through the above evaluation, we will be able to find out which time range gives the best prediction for each possible model by implementing feature engineering on the given dataset.


### 10. Additional Resources
**A list of resources you have/need to conduct the project. This includes additional reading, software, datasets, code (Github link), etc., beyond your chosen dataset. Are these resources public? How are you planning to get these resources?**

**Rubric: 
a) Does the proposal give a short list of resources the team plans to use to execute the project (inclusive of readings, software, datasets, etc.)?
b) Does the team describe any strategy for getting the resources?**

- Our team decides to use the following resources. They are all available online and they are public. The resources can be found in the links below.
    - Towards Data Science: https://towardsdatascience.com/
    - Analytics Vidhya: https://www.analyticsvidhya.com/
    - Investopedia: https://www.investopedia.com/
    - Trading View (reference for technical analysis tools): https://www.tradingview.com/chart
    - Software used: Google Colab
    - Visualisation tools: Python libraries, such as Matplotlib, seaborn
    - Recent stock data (2017 to 2020): https://www.kaggle.com/jacksoncrow/stock-market-dataset
 
### 11. Schedule / Role Assignment
**A schedule of work indicating the dates by which you plan to complete components of the project. Make sure the schedule is plausible.
You may find that a table format with the remaining weeks of the course helpful to describe this goal.**

**Rubric:
a) A schedule indicating dates by which the team plans to complete the project components?
b) An assignment of the team members to the deliverables (inclusive of peer reviewing duties)?
c) Is the schedule feasible given the timeline, expertise and load of the team members?
d) For projects with large data sources, does the team propose a way to scope the data or problem accordingly to make it feasible?**

- Tentatively, we plan to work on all tasks together (including peer review) as a team. We will meet twice weekly (every Wednesday and Saturday) to discuss the tasks and split the subtasks and update the specific roles if necessary.
- General timeline: 
  - Week 4 (29/8 - 4/9) - Research on project topics & dataset
  - Week 5 (5/9 - 11/9) - Discuss and decide dataset that we are using, finalise proposal
  - Week 6 (12/9 - 18/9)- Research on possible ways of data transformation to aid in time series model prediction
  - Week 7 to 10 (26/9 - 23/10) - Build possible models (Linear Regression, k-Nearest Neighbors, Auto ARIMA etc)
  - Week 11 to 13 (24/10 - 13/11) - Fine-tuning the models, model evaluation, decide final model

- *Since our data only consists of 8.4k text files of small size, no scoping of problems is needed.*


