# Twitter Keyword Corpus

## Description

The Twitter dataset consists of English tweets from Twitter posted on April 2011. 
The tweets have been assigned keyphrases by humans through the Amazon Mechanical Turk platform. 
Each tweet was evaluated by three assigners, where each assigner had to choose between 1 and 4 keyphrases for each evaluated tweet.
The final set of keyphrases selected for each tweet was made by selecting only those terms that had an agreement ratio of at least 2/3.

## Format

Two files are provided:
1. **Twitter Keywords:** `twitter_keywords.csv`
2. **Twitter Texts:** `twitter_texts.csv`

### Twitter Keywords
Fields:
* `document_id`: The id of the tweet (matches with an id in the texts file)
* `keyword`: A keyword belonging to that tweet

### Twitter Texts
Fields:
* `document_id`: The id of the tweet (matches with an id in the keywords file)
* `category`: The source of this tweet
* `original_text`: The original tweet text
* `stemmed_text`: The lemmatized tweet text
* `word_count`: The number of words in the tweet
* `keyword_percentage`: The percentage of assigned keywords that actually appear in the tweet (0-1)