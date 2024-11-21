# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: APIs, NLP, and Classification

### Description

In weeks five and six, we learned about various classifiers and their corresponding metrics. In week seven, we'll learn about APIs and Natural Language Processing (NLP) and then put those skills to the test.

For project 3, your goal is two-fold:
1. Using Reddit's API, you'll collect posts from two subreddits of your choosing.
2. You'll then use NLP to train classifiers on which [subreddit](https://reddit.zendesk.com/hc/en-us/articles/204533569-What-are-communities-or-subreddits-) a given post came from. This, as you're well aware, is a binary classification problem.


#### About the API

Reddit's API is fairly straightforward. For example, if I want the posts from [`/r/boardgames`](https://www.reddit.com/r/boardgames), all I have to do is add `.json` to the end of the url: https://www.reddit.com/r/boardgames.json

<!-- To help you get started, we have a primer [video](https://www.youtube.com/watch?v=5Y3ZE26Ciuk) on how to use Reddit's API. -->

---

### Requirements

- Gather and prepare your data using the `requests` library or use the code provided by the instructional team.
- **Create and compare _at least_ two models**. One of these must be a Naive Bayes classifier, however the other can be a classifier of your choosing: [Logistic Regression](https://scikit-learn.org/1.5/modules/generated/sklearn.linear_model.LogisticRegression.html), [KNN](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html), [Random Forest](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html), [Gradient Boosting](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.GradientBoostingClassifier.html), [XGBoost](https://xgboost.readthedocs.io/en/stable/), etc. 
- **You are of course encouraged to test out more than two classifiers**. 
- A well-commented, well-documented Jupyter Notebook with your analysis for a peer audience of data scientists.
- An executive summary of the results you found.
- A presentation outlining your team's process and findings for a (mostly) technical audience.

**Pro Tip 1:** You can find a good example of an executive summary [here](https://www.proposify.biz/blog/executive-summary).

**Pro tip 2:** The API will cap you at 1,000 posts for each subreddit (**assuming the subreddit has that many posts**).

---

### Necessary Deliverables / Submission

- Code and executive summary must be in a clearly commented Jupyter notebook (or notebooks).
- Your project team's presentation slides.
- All project materials, with the exception of your presentation slides, must be submitted no later than **9am on Thursday, November 21st, 2024**.
- Your presentation slides must be submitted by **9am on Friday, November 22nd, 2024**.

---

## Rubric
Your instructional team will evaluate your project using the following criteria.  You should make sure that you consider and/or follow most if not all of the considerations/recommendations outlined below **while** working through your project.

For Project 3, the evaluation categories are as follows:<br>

**The Data Science Process**
- Problem Statement
- Data Collection
- Data Cleaning & EDA
- Preprocessing & Modeling
- Evaluation and Conceptual Understanding
- Conclusion and Recommendations

**Organization and Professionalism**
- Organization
- Visualizations
- Python Syntax and Control Flow

**Presentation**


### The Data Science Process

**Problem Statement**
- Is it clear what the goal of the project is?
- What type of model will be developed?
- How will success be evaluated?
- Is the scope of the project appropriate?
- Is it clear who cares about this or why this is important to investigate?
- Does the student consider the audience and the primary stakeholders?

**Data Collection**
- Was enough data gathered to generate a significant result?
- Was data collected that was useful and relevant to the project?
- Was data collection and storage optimized through custom functions, pipelines, and/or automation?
- **_Was thought given to the server receiving the requests such as considering number of requests per second?_**

**Data Cleaning and EDA**
- Are missing values imputed/handled appropriately?
- Are distributions examined and described?
- Are outliers identified and addressed?
- Are appropriate summary statistics provided?
- Are steps taken during data cleaning and EDA framed appropriately?
- **_Does the project team address whether or not they are likely to be able to answer their problem statement with the provided data given what they've discovered during EDA?_**

**Preprocessing and Modeling**
- Is text data successfully converted to a matrix representation?
- **Are methods such as stop words, stemming, and lemmatization explored?**
- Does the project team properly split and/or sample the data for validation/training purposes?
- Does the project team test and evaluate a variety of models to identify a production algorithm (**AT MINIMUM:** Naive Bayes and one other model)?
- **_Does the project team defend their choice of production model relevant to the data at hand and the problem?_**
- **_Does the project team explain how the model works and evaluate its performance successes/downfalls?_**

**Evaluation and Conceptual Understanding**
- Does the project team accurately identify and explain the baseline score?
- Does the project team select and use metrics relevant to the problem objective?
- Does the project team interpret the results of their model for purposes of inference?
- Is domain knowledge demonstrated when interpreting results?


**Conclusion and Recommendations**
- Does the project team provide appropriate context to connect individual steps back to the overall project?
- Is it clear how the final recommendations were reached?
- Are the conclusions/recommendations clearly stated?
- **_Does the conclusion answer the original problem statement?_**
- Does the project team address how findings of this research can be applied for the benefit of stakeholders?
- **_Are future steps to move the project forward identified?_**


### Organization and Professionalism

**Project Organization**
- Are modules imported correctly (using appropriate aliases)?
- Are data imported/saved using relative paths?
- Does the README provide a good executive summary of the project?
- Is markdown formatting used appropriately to structure notebooks?
- Are there an appropriate amount of comments to support the code?
- Are files and directories organized correctly?
- Are there unnecessary files included?
- Do files and directories have well-structured, appropriate, consistent names?

**Visualizations**
- Are sufficient visualizations provided?
- Do plots accurately demonstrate valid relationships?
- Are plots labeled properly?
- Are plots interpreted appropriately?
- Are plots formatted and scaled appropriately for inclusion in a notebook-based technical report?

**Python Syntax and Control Flow**
- Is care taken to write human readable code?
- Is the code syntactically correct (no runtime errors)?
- Does the code generate desired results (logically correct)?
- Does the code follows general best practices and style guidelines?
- Are warning handled in an appropriate manner?
- Are Pandas functions used appropriately?
- Are `sklearn` and `NLTK` methods used appropriately?

**Presentation**
- Is the problem statement clearly presented?
- **_Does a strong narrative run through the presentation building toward a final conclusion?_**
- **_Are the conclusions/recommendations clearly stated?_**
- Is the level of technicality appropriate for the intended audience?
- Is the presentation substantially over or under time?
- Does the project team appropriately pace their presentation?
- **_Do the members of the project team deliver their message with clarity and volume?_**
- Are appropriate visualizations generated for the intended audience?
- Are visualizations necessary and useful for supporting conclusions/explaining findings?


---

### Why did we assign this project to you?
This project covers three of the biggest concepts of the class: Classification Modeling, Natural Language Processing, and Data Wrangling/Acquisition.

Part 1 of the project focuses on **Data wrangling/gathering/acquisition**. This is a very important skill as not all the data you will need will be in clean CSVs or a single table in SQL.  There is a chance that wherever you land you will have to gather some data from some unstructured/semi-structured sources; when possible, requesting information from an API.

Part 2 of the project focuses on **Natural Language Processing** and converting standard text data (like Titles and Comments) into a format that allows you to analyze it and use it in modeling.

Part 3 of the project focuses on **Classification Modeling**.  Given that project 2 was a regression focused problem, we wanted to give you a classification focused problem to practice the various models, means of assessment, and preprocessing associated with classification.
