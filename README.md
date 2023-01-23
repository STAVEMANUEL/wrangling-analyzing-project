## wrangling-analyzing-project
gathered, assessed, clean and analyze WeRateDog twitter user using: Python 

WeRateDogs Twitter data was retrieved from Twitter's API using Tweepy, a Python library. Among the data will be the number of retweets and favorites. As part of this project, I combined those two pieces of data with additional information provided by Udacity's Data Analyst course. During the process of Data Wrangling of tweet data from the Twitter user @dog_rates , I have found several quality and structure issues. After analyzing, cleaning, and combining all the data, I have created a new DataFrame. I have stored it in twitter_archive_master.csv.

With the link provided by Udacity, I downloaded and imported the WeRateDogs Twitter archive .
Using Python's Requests library, I downloaded the tweet image predictions file hosted on Udacity's servers and saved it locally as image_predictions.tsv. Next, I imported this file into a Python Pandas dataframe.
Scrolling through the twitter_archive_enhanced.csv and image_predictions.tsv files in Excel, I looked for tidiness and quality problems.

As part of my analysis i used info method to identify erroneous datatypes and other quality issues. In order to verify i used value counts method in test fields.

Assessing Data
the timestamp is object - it should be datetime.

not all tweets about dogs.

there is url inside text.

no need for retweets

there are 546 none values in column "name" and also 55 "a" names which is incorrect.

retweet and favorite count are float datatype.

the source column is with 3 values , aranged as html code.

the source are object datatype and not a category.
