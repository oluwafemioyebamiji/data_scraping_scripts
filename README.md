# data_scraping_scripts
Documentation for Data Extraction Engine to Fetch Information from News Channels and Twitter
January 2021.

1.0.	Introduction
With a need to fetch mentions of keywords from across several news channels and twitter, this python scripts attempt to automate the process. The code is written in python programming language using Jupyter notebook.

2.0.	Scripts Location:
•	NEWS CHANNELS SCRIPT GITHUB URL: https://github.com/oluwafemioyebamiji/data_scraping_scripts/blob/master/News_Scrape_Script_newsapi.ipynb

•	TWITTER SCRIPT GITHUB URL: https://github.com/oluwafemioyebamiji/data_scraping_scripts/blob/master/Tweet_Scrape_Script.ipynb

3.0.	Documentation A: Twitter News Fetching Script
This script fetches mentions of keywords from twitter. The following steps are required for the running of this script:
1.	Supply your twitter developer account details in the second cell:
TWITTER_CONSUMER_KEY
TWITTER_CONSUMER_SECRET
TWITTER_ACCESS_TOKEN TWITTER_ACCESS_TOKEN_SECRET
You can create an account and get your developer account details at https://developer.twitter.com/en/apply-for-access. Default used for testing this script is a personal key of Femi Oyebamiji.
2.	Modify only the last section of the code -
A.	search_words: The keywords to search. You can use the keyword "AND" if you want to fetch only where the two
keywords appear. "OR" for if any of the keyword exist. E.g., Endsars OR Covid.
B.	date_since: The specific start date of the tweet you want to fetch,
C.	numTweets: The number of tweets to fetch per run - best at 2500 maximum for a free account,
D.	numRuns: For example if you need 10,000 mentions, you can set this to 4 for a 2500 per numTweets.
3.	Run the script: Click on the last code section and press shift key + enter key at the same time on a jupyter notebook.
The result is automatically outputted to an external excel/csv sheet in the data folder named TWEETS_timetamp.csv
This script can also be integrated into a software solution.

4.0.	Documentation A: Twitter News Fetching Script
This script fetches mentions of inputed keywords from across over 50 news channels using the NewsAPI. The following steps are required for the running of this script:
1.	Supply your NewsAPI key - This can be obtained on https://newsapi.org. The default used for testing this script is a personal key of Femi Oyebamiji. This script will be able to work with the free version of the NewsAPI key. However, you can only access news published within the last one month with the free key.
2.	Modify only the last section of the code -
A.	Topic News: The keywords to search which can be separated with comma,
B.	from_date: The specific start date of the news you want to fetch,
C.	to_date:  the end date of what you want to fetch,
D.	language: The language of the news to fetch. Default is English.
3.	Run the script: Click on the last code section and press shift key + enter key at the same time on a Jupyter notebook.
The result is automatically outputted to an external excel/csv sheet in the data folder named current_timestamp + NEWS.csv
This script can also be integrated into a software solution.

5.0.	Need help?
Reach out to Femi Oyebamiji – +2348160837781
