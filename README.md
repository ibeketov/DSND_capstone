# Sparkify project

### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [Files Description](#files)
4. [Result](#Result)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

This project uses the following software and Python libraries:

- Python
- Spark
- Pyspark
- pandas
- Seaborn

You will also need to have software installed to run and execute a Jupyter Notebook.

If you do not have Python installed yet, it is highly recommended that you install the Anaconda distribution of Python, which already has the above packages and more included. And for Spark, you can do this using AWS or IBM Cloud.

Please check the requirements.txt for complete information about working environment.

Please use `pip install -r requirements.txt` to run it

## Project Motivation<a name="motivation"></a>

This is udacity's capstone project, using spark to analyze user behavior data from music app Sparkify.

Sparkify is a music app, this dataset contains two months of sparkify user behavior log. The log contains some basic information about the user as well as information about a single action. A user can contain many entries. In the data, a part of the user is churned, through the cancellation of the account behavior can be distinguished.

## Files Description<a name="files"></a>

**Sprakify .ipynb** Main file of the project, it demonstrates the process of using pyspark to explore the data and build the model.

## Result

In this project first I introduced three baseline algorithms in order to predict customer churn rates of a Sparkify app. The best performing one was the gardient boosting algorithm with an Accuracy of over 83% and F1 score of 81%.

Second, based on its performance I proceeded with gradient boosting algorithm. Additionally in the second step I applied hyperparameter tuning via grid search. The reason for this strategy is the assumption, that gradient bosting will, despite overfitting, perform best on the wohle dataset.

After the second run of the garadient boosting with hyperparameter tuned, the results are similar to those from the baseline model. The F1 score remained very high at 80%. As a next step we should test gradient boosting on the entire dataset.

Furthermore, I also examined the most important factors for the churn rate as it is displayed in the feature importance section. The most important factors in customer churn seem to be: the number of songs played per user, user engagement as represented by the thumbs up/down feature and overall listening time.

I post a blog about the detail, you can find it [here](https://ibeketov.github.io/DSND_capstone/).

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

Must give credit to Udacity for the project. You can't use this for you Udacity capstone project. Otherwise, feel free to use the code here as you would like! 
