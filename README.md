# Starbucks Capstone Challenge

## Installation:

* Python Libraries:
* Pandas.
* Scikit-learn.
* numpy.
* time.
* matplotlib.
* seaborn.

## Introduction:

This data set contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks.
Not all users receive the same offer, and that is the challenge to solve with this data set.

## Data Sets:

The data is contained in three files:
* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
* profile.json - demographic data for each customer
* transcript.json - records for transactions, offers received, offers viewed, and offers completed

## Data understanding:

#### portfolio.json:
* id (string) - offer id
* offer_type (string) - type of offer ie BOGO, discount, informational
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) - time for offer to be open, in days
* channels (list of strings)

#### profile.json:
* age (int) - age of the customer
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income

#### transcript.json:
* event (str) - record description (ie transaction, offer received, offer viewed, etc.)
* person (str) - customer id
* time (int) - time in hours since start of test. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record

## Problem Statement:

* What is the Gender Distribution of Starbucks Customers?
* What is the Age Distribution of Starbucks Customers?
* What is the Income Distribution of Starbucks Customers?
* How many customers enrolled yearly?
* Which gender has the highest yearly membership?
* Which gender has the highest Annual income?
* What is the distribution of event in transcripts?
* What is the percent of trasactions and offers in the event?
* What is the Income Distribution for the Offer Events?
* What are the Offer types amongst ages, gender and income groups?

## Conclusion:

On analysis the data using supervised and unsupervised learning(Kmeans), we can conclude that:

Different segments of customers react to offers differently.
The count of male customers in low-income level is slightly higher than that of female and other customers
Though the average salary of female is greater than that of the male, female spend less on Starbucks than male
Starbucks has more of the young crowd than those of the aged once.
The result of the offer_type was predicted by training a supervised classifier.

## Results:

Customers are attracted to BOGO and Discount offers more as compared to Informational Offers
The buying behavior of a customer is independent of its annual income
Starbucks have more male customers than females and other gender.
KNeighborsClassifier turned out to be the best algorithm for this task and predicts customer response with an accuracy rate of almost % after hyperarameter tuning. Given the fact that also the same customer will react differently the same offer.

## Blog:
