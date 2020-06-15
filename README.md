# edinburgh-airbnb-may2020
Investigation of the factors influencing price and popularity of properties on Edinburgh AirBnB.


## Libraries

Only standard anaconda python libraries are used, namely:
* pandas
* matplotlib.pyplot
* seaborn
* nltk
* sklearn

## Motivation

This project investigates AirBnB Edinburgh data, investigating the factors that affect the price and popularity (number of bookings in the next 90 days) of listed properties.

Note: This project forms part of Udacity's Data Scientist Nanodegree programme.

## Process and Methodology
Below is the process followed in the analysis.

### Business Understanding
I want to analyse the factors that affect the price and popularity of Edinburgh listings on Airbnb. Specifically,
I want to look at the following four questions:
1. How much of an effect does neighbourhood have?
2. How much of an effect do reviews have?
3. How much of an effect do host qualities have?
4. Can a machine learning model be effectively used to see what other attributes have an effect?

### Data Understanding
This process is done at the beginning of the project (section 2. Investigating Target Columns), and repeated for all 4 business questions. The most effective columns for the question at hand are investigated and evaluated.

### Prepare Data
Like the Data Understanding step, preparing the data is done at the beginning of the project for target columns, and repeated for each new question as further columns need to be pulled into the analysis. Missing values are filled in, columns are converted into a usable form, and features are engineered.

### Data Modeling
This step is processed separately for each business question. In the case of the first three, this takes the form of gathering statistics and individual linear regression charts. For the fourth question, this takes the form of creating a full Linear Regression model.

### Evaluate the results
This step is carried out at the end of every business question step. The modelled data is evaluated to find correllations, and the Linear Regression model's performance is assessed to see if it can provide useful insight.

## Files

* 'listings.csv.gz' contains data on Edinburgh AirBnB properties, as compiled on 27th May, 2020.
* 'AirBnB Edinburgh Data Investigation.ipynb' contains all of the code investigating the data.

## Summary of Results

Neighbourhood strongly correlates with price and popularity, with the more affluent, central areas of Edinburgh being both more expensive and more popular.

Properties with no reviews tend to be a little more expensive. Properties with a high number of reviews tend to be more popular, but also slightly less expensive. However, the actual rating of the review doesn't correlate strongly with either price nor popularity.

Hosts with a profile picture tend to charge more per bedroom, and superhosts are more popular than non-superhosts.

A linear regression machine learning model did not provide useful insight with this dataset, not performing well even on the training data.


## Acknowledgements

Thanks to Inside AirBnB for the data, you can find a link to their full resource [here](http://insideairbnb.com/get-the-data.html).

Thanks to the Names Corpus from the nltk libary, authored by Mark Kantrowitz and Bill Ross (see entry 43 [here](https://www.nltk.org/nltk_data/)).
