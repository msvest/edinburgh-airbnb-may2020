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

This project investigates AirBnB Edinburgh data, investigating the factors that affect the price and popularity of listed properties.

Specifically, I look at neighbourhood, reviews, and the host, to see what effect they have on property price and popularity. I also make a Linear Regression model to see if there are other factors that influence price and popularity.

Note: This project forms part of Udacity's Data Scientist Nanodegree programme.

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
