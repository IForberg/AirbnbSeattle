# AirbnbSeattle

This project is part of an assignment in Udacity's Data Scientist for Enterprise nanodegree. I have been looking at data from Seattle Airbnb found at https://www.kaggle.com/airbnb/seattle/home and done some analysis of the main dataset based on three questions:
- Can a linear regression model accurately predict the list price of a property?
- What are the top amenities that should be included in a property to get the best price and what should be dropped?
- Can an automatic machine learning tool like TPOT do an equally good job creating a predictive model as the linear regression model in quetion 1? In other words, is it possible for a company with little background in machine learning to reap some of the benefits from the field by using auto-ml packages like TPOT?


## Summary

The linear regression model found had an r-squared of 0.6. This could be better but still not bad as a starting point.

The three most important amenities determining price were having a doorman, a hot tub and an elevator in the building. The three amenities that actually led to a lower price where a washer/dryer onsite, hangers(!) and the availability of 24-hour check-in. Most of these findings implies that the adage that correlation does not mean causation.

Letting TPOT, an auto-ml package, work on the dataset for two minutes led to a model using the random forest algorithm that increased the r-squared to 0.65. This implies that auto-ml packages should not be discounted when doing machine learning.


## Installing

Anaconda with Python 3.6 was used for completing the project.
TPOT is not part of the standard Anaconda libraries and can be installed using conda: `conda install -c conda-forge tpot`
More information about TPOT can be found at https://github.com/EpistasisLab/tpot


## Files

The jupyter notebook, source files and one output file are included in this repository.


## Blog post

A blog post describing the results can be found at
