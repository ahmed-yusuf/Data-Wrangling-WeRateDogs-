## A Data-Wrangling project as part of Udacity's Data Analysis Nanodegree

## OVERVIEW

WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has over 8 million followers and has received international media coverage.

Please check Dogs Are Doggos: An Internet Language Built Around Love For The Puppers to familiarize yourself with formal Doggolingo as you will see much use of it in this analysis

For more on dog breeds, please check DogTime. Also, all breed info were collected and stored in a separate CSV file for your convenience.

## Table of Content
* Introduction
*Gather Data
*Assess the Data
*Clean the Data
*Analysis
*Conclusions


### Data Gathering:
This project required gathering three data sets. The method used to gather each data was different and are as follows.

Twitter archive file: This can be downloaded manually or programmatically with the use of the Request library

The tweet image predictions: This can only be downloaded programmatically using the Request library because the file image_predictions.tsv is hosted on Udacity's servers and cannot be accessed manually.

Tweets: Each tweet's retweet count and favorite ("like") count at minimum, and any additional data found to be interesting are scraped. This is done by:

Extracting the tweet IDs in the WeRateDogs Twitter archive and store in another file (tweet_id.txt)
Quering the Twitter API for each tweet's JSON data using Python's Tweepy library and store the data in another file (tweet_json.txt)

#### Data Wrangling

1.Twitter_archive file contains name column contains none values.

2.Some names in twitter_archive name column arent actual names of individuals.

3.Some twitter_archivecopy columns has a different filetype e.g the timestamp column is seen as an object type.

4.No column for month or year for easy analysis.

5.Too many redundant columns that can be combined into dog_stage.

6.Not all values in the image_predictions dataset has .jpg extension.

7.Delete unusual column

8.Rearrange columns for easy matching.

9.Remove columns that wont be used for analysis.

TIDYNESS ISSUES
1.Merge data frames on their shared tweet_ids.

2.There are a lot of null values in the columns doggo, floofer, puppo, and pupper.

Exploratory D

### Requirements

* Jupyter Notebook
*Pandas
*Numpy
*Requests
*Tweepy
*json
*Matplotlib


```python

```
