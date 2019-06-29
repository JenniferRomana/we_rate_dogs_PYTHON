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
import numpy as np
import pandas as pd
import requests
import os
import tweepy
import wptools
import json
from timeit import default_timer as timer
import matplotlib.pyplot as plt
import seaborn as sns
