# TwittTrends
The TwittTrends app is to show tweets location on the Google Map and indicate the sentiment associated with the tweet.

The green markers are used to indicate positive sentiment.

The blue markers are used to indicate neutral sentiment.

The red markers are used to indicate negative sentiment.


We use Elasticsearch to store the data, ElasticBeanstalk to deploy the application.

SQS and SNS service are used to implement the tweet queue, process the tweets for their corresponding sentiment using AlchemyLanguageV1 API and notify the web application about the new tweets arrived and ready to be indexed into elastic search.


Python Flask framework is used to implement the application.
