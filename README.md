# Starbucks_Capstone_Project
Starbucks Capstone Project for Udacity DSND

## Table of Contents
1. [Description](#description)
2. [Requirements](#requirements)
3. [Materials](#materials)
4. [Acknowledgement](#acknowledgement)
5. [Additional Details](#details)

<a name="descripton"></a>
## Description
This Capstone Project is a requirement under Udacity DSND Program.
In this project, we are trying to "Measure Marketing Campaign Effectiveness" using a data that mimics the Starbucks Reward mobile App data.
The data set provided, entails simulated data that mimics customer behavior on Starbucks rewards mobile app. 
Customers using Starbucks mobile app receive random offers from Starbucks, the offer might range from merely an informational offer advertising about a drink, to an discount offer that a customer can avail on their spending's at Starbucks, or a BOGO (Buy One Get One) offer.
All these offers are time bound with a designated expiry. The customers are rewarded based on their cumulative spend activity during the period in which offer was active. The offers are sent to customers in no particular order, some customers might not receive any offer, while not all user receive the same offer.

#### Data sets

The data is contained in three files:

* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
* profile.json - demographic data for each customer
* transcript.json - records for transactions, offers received, offers viewed, and offers completed

Here is the schema and explanation of each variable in the files:

**portfolio.json**
* id (string) - offer id
* offer_type (string) - type of offer ie BOGO, discount, informational
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) - time for offer to be open, in days
* channels (list of strings)

**profile.json**
* age (int) - age of the customer 
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income

**transcript.json**
* event (str) - record description (ie transaction, offer received, offer viewed, etc.)
* person (str) - customer id
* time (int) - time in hours since start of test. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record


<a name="requirements"></a>
## Requirements
* Python 3.5+
* Machine Learning Libraries: NumPy, SciPy, Pandas, Sciki-Learn
* Data Visualization Libraries: Matplotlib, Seaborn
* Json to read the json files

<a name="materials"></a>
## Materials
1. **Starbucks_Capstone_notebook.ipynb Notebook**: Notebook containing the full analysis of the Starbucks Capstone Project.
2. **cust_data_clean.csv**: The csv file conatining the cleaned transcript data.
3. **Data** : Folder containing original datasets.

<a name="acknowledgement"></a>
## Acknowledgements
* [Udacity](https://www.udacity.com/) and Starbucks for providing such a wonderful project

<a name="details"></a>
## Additional Details

1.Blog post : The blog post in Medium can be found  here https://medium.com/@smithathalur/measuring-marketing-campaign-effectiveness-using-starbucks-reward-mobile-app-data-5456c8e5ad45

