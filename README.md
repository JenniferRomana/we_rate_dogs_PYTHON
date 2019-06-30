# WeRateDogs - Data Wrangling and Analysis

*WeRateDogs* is a Twitter account that gives humourous comments and ratings of
people's dogs.  It has over 8 million followers and international media coverage.

The data is assessed both visually and programatically to find any quality or
tidiness issues.
- Quality issues relate to the data content and
- Tidiness issues relate to the structure of the data.
Each issue is then in turn treated and cleaned.

Finally the data is explored, guided by question

How do the Dog Rating Tweets relate to the popularity and phenomenal success of
*WeRateDogs* Twitter account?

### Datasets
1. File on hand: `twitter-archive-enhanced.csv`
- WeRateDogs Twitter archive supplied by Udacity
- includes basic tweet data for over 2,000 tweets that have ratings
2. File from the internet:  `image_predictions.tsv`
- prediction file that gives the top 3 predictions of a dog's breed based on
a jpeg image associated with each tweet that has been run through a neural network.  
- This file is hosted on Udacity's server
https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsvImage
3. Twitter API data: `tweet_json.txt`
- query Twitter's API using Tweepy and save the JSON data to text


### Imports
import numpy as np<br>
import pandas as pd<br>
import requests<br>
import os<br>
import tweepy<br>
import wptools<br>
import json<br>
from timeit import default_timer as timer<br>
import matplotlib.pyplot as plt<br>
import seaborn as sns<br>

### How to Query Twitter API
You will need to set up your own Twitter application in order to query Twitter API.

1. Sign up for Twitter account
2. Apply for a Developer account
3. Set up a Twitter application and generate Consumer API keys, Access Token and
Access Token secrets

#### creds.py
Create a creds.py python file containing API keys and Tokens.  A sample file is
included in the repository.  

The Jupyter notebook wrangle_act.ipynb will import this file in the section
**Gather 3. Twitter's API data**

#### Make sure to .gitignore this creds.py file


**If you do not wish to open a Twitter account or query the Twitter API**,
a copy of the tweet_json.txt file is included in the data folder of
this repository.  For the Gather 3. Twitter's API data section,
you may then just run the code from the cell starting with <br>
*# Read json_tweet.txt line by line to extract tweet_id, retweet_count and favourite_count*
