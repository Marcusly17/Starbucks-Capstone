# Starbucks-Capstone
Udacity Data Science Nanodegree Capstone Project

## About Project

Starbucks provided simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks. Not all users receive the same offer.

### Problem Statement

1. Whether a customer will respond the offer based on the demographics and offer type?
2. What are the most important factors affecting customers' response?

### Summary of Analysis

- By using random forest model, customers' response can be predicted by their demographics and the offer type. 

- The amount of spending without offer and the length of membership are the top two most important factors when customers decide whether to respond the offer.

- The social media is the most important channel to deliver offer to customers.

- Reward and duration are the fourth and fifth important features. If reward is too low and the duration is too short, it's hard for customers to respond the offer.

## Getting Started

### Installation

- The code should run with no issues using Python version 3.*.
- Libraries used: Numphy, Scipy, Pandas, Sciki-Learn, Matplotlib, Seaborn

### File Description

The data is contained in three files:

- portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
- profile.json - demographic data for each customer
- transcript.json - records for transactions, offers received, offers viewed, and offers completed

Here is the schema and explanation of each variable in the files:

**portfolio.json**

- id (string) - offer id
- offer_type (string) - type of offer ie BOGO, discount, informational
- difficulty (int) - minimum required spend to complete an offer
- reward (int) - reward given for completing an offer
- duration (int) - time for offer to be open, in days
- channels (list of strings)

**profile.json**

- age (int) - age of the customer
- became_member_on (int) - date when customer created an app account
- gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
- id (str) - customer id
- income (float) - customer's income

**transcript.json**

- event (str) - record description (ie transaction, offer received, offer viewed, etc.)
- person (str) - customer id
- time (int) - time in hours since start of test. The data begins at time t=0
- value - (dict of strings) - either an offer id or transaction amount depending on the record

## Acknowledgements

Data for coding project was provided by Udacity

## Blog 

The detailed explanation and exploration are published on medium [here](https://medium.com/@3nh/starbucks-capstone-challenge-31095852630c).
