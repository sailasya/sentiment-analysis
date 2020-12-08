**Sentiment Analysis**

_**Technologies & Libraries used :**_

`1. Python
2. NLTK 
3. numpy
4. pandas
5. tweepy` 

Throughout this project, focus is on a challenging problem of detecting emotional state of a person based on his/her interactions on social media platforms, in this  twitter. 
The main contributions of work are as follows:

1.Data labeling has been done using the ground-level truth sentence patterns like “I feel sad, happy etc”. This method of data labeling has reduced the human effort to
manually label the data sets.

2.A variety of statistical attributes like behavioral attributes, social engagement and linguistic style attributes from users’ sampling period tweet postings have been proposed.

The results obtained showed that proposed model is effective and efficient on detecting emotional state of user from micro-blog data.

Below are the steps followed :

_**1. Data Collection :**_ 

Twitter's official Twitter APIs for developers are used to collect publicly available tweets. There are many tools that use the official APIs to collect data. 

Following items are used to collect raw tweets.

`1) Python 
2) Tweepy 
3) Access Tokens given by Twitter APIs.`

Tweepy, a python library that use Twitter APIs is used in this project.

_**2. Data Preprocessing :**_ 

Twitter REST APIs which are sufficient enough to collect required tweets data.

Data extraction using python and tweepy. Steps involved in collecting raw tweets data :

_Get access Tokens from Twitter APIs: _

In order to access twitter REST APIs, one needs to get access tokens from Twitter APIs. There are four tokens to be taken from Twitter APIs to collect required tweets data. They are :

a) Consumer Key, b) Consumer Secret, c) Access Token and d) Access Token Secret.

`Following are the steps to get the four tokens.

1) Go to https://apps.twitter.com/ and log in with your twitter credentials.

2) Click on “Create New App” button.

3) Complete the form, check the “agree to the terms” check box and click on “Create your Twitter application” Button

4) In the next page, click on “API keys” tab, and copy the application’s “API key” and “API secret”.

5) Scroll down and click “Create my access token”`

_Collect tweets data:_

In order to collect data, one needs to select the twitter users whose tweets are being collected. Selected two set of users who are active in twitter and then collected their tweets for a period of four months. Total number of tweets collected is around 40,000. Following is the code snippet to collect data for a specific user.

All the tweets collected are stored in organized structured format.

_**3. Data Preprocessing :**_

Twitter is considered as a source for data. For data processing, first one needs to get raw tweets data from twitter. Secondly, pre-processing and extraction of features from the raw tweets are done for observation and analysis.

Data Preprocessing involves following steps :

Removal of URLs in tweet text
Removal of emoticons
Removal of punctuations
Tokenizing the sentences
Removal of stop words as they do not contribute to polarity
Parts of speech tagging of the sentences
Count of positive and negative polarity words
Grouping these modified tweets by user screen name or id

_**4. Data labeling :**_

Tweets are labeled as positive tweet (1), negative tweet(-1) and neutral tweets(0) based on the common sentence patterns that expresses the emotion of a person such as , “I feel happy”, “ I feel stressed” etc., This method of labeling is proved to be effective in emotional analysis . Now data is available for feature extraction, analysis, further processing. Datasets Summary Collected 51 users tweet data from 01.2018 to 04.2018 as dataset1 and 62 users tweet data from 11.2017 to 02.2018 as dataset2. 

Details of the datasets are summarized in tables

Dataset 1: Collected 51 users tweet data from 01.2018 to 04.2018 as dataset1

Dataset-1

Label Positive Negative Neutral

No of tweets 36507 14423 44719

Average Number of Tweets per user 715.8235 282.8039 876.8431

Average Number of Tweets per day 165.19 65.2624 202.3484

Average Number of Tweets per week 1106.273 437.0606 1355.121

Average Number of Tweets per user per day 7.5993 3.0023 9.3087

Average Number of Tweets per user per week 42.0104 16.5972 51.4603
