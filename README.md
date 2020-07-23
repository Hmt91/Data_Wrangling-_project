# Data_Wrangling-_project
Wrangling data from WeRateDogs Twitter account 

# My goal:
wrangle WeRateDogs Twitter data to create interesting and trustworthy analyses and visualizations.

# Data Overview:  
The Twitter archive is great, but it only contains very basic tweet information. Additional gathering( Twitter APIs , online files ..etc), then assessing and cleaning is required for neat analyses and visualizations. 
### • Enhanced Twitter Archive :
       The WeRateDogs Twitter archive contains basic tweet data 2356 tweets . 
       tweet_id: the unique identifier for each tweet  
       in_reply_to_status_id: if the represented Tweet is a reply, this field will contain the integer representation of the original Tweet’s ID  
       in_reply_to_user_id: if the represented Tweet is a reply, this field will contain the integer representation of the original Tweet’s author ID 
       timestamp: time when this Tweet was created 
       source: utility used to post the Tweet, as an HTML-formatted string. e.g. Twitter for Android, Twitter for iPhone, Twitter Web Client 
       text: actual UTF-8 text of the status update 
       retweeted_status_id: if the represented Tweet is a retweet, this field will contain the integer representation of the original Tweet’s ID 
       retweeted_status_user_id: if the represented Tweet is a retweet, this field will contain the integer representation of the original Tweet’s author ID
       retweeted_status_timestamp: time of retweet 
       expanded_urls: tweet URL 
       rating_numerator: numerator of the rating of a dog. Note: ratings almost always greater than 10 
       rating_denominator: denominator of the rating of a dog. Note: ratings almost always have a denominator of 10 
       name: name of the dog 
       doggo: one of the 4 dog "stage" 
       floofer: one of the 4 dog "stage" 
       pupper: one of the 4 dog "stage" 
       puppo: one of the 4 dog "stage"
	
  ### •	Image Predictions File :
        a table full of image predictions 
        tweet_id | is the last part of the tweet URL 
        p1 |is the algorithm's prediction for the image in the tweet 
        p1_conf | is how confident the algorithm is in its prediction 
        p1_dog | is whether or not the prediction is a breed of dog 
        p2 | is the algorithm's second most likely prediction 
        p2_conf | is how confident the algorithm is in its prediction 
        p2_dog | is whether or not the prediction is a breed of dog 

### In my wrangling I will follow this Key points:
• I only want original ratings (no retweets) that have images.  
• The requirements of this project are only to assess and clean at least 8 quality issues and at least 2 tidiness issues in this dataset.  
• The fact that the rating numerators are greater than the denominators does not need to be cleaned. This unique rating system is a big part of the popularity of WeRateDogs)  
• I do not need to gather the tweets beyond August 1st, 2017 becouse won't be able to gather the image predictions for these tweets since I don't have access to the algorithm used.
