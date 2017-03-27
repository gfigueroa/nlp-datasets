Document collections used in "RankUp: Enhancing Graph-Based Keyphrase Extraction Methods with Error-feedback Propagation"
===============================================================================

# Description of the collections

Four different document collections were used in our experiments, adding up to a total of 4,607 texts. In each collection, with the exception of the Hulth 2003 corpus, 50% of the documents were randomly selected and used for validation (i.e. selecting the best parameter values for RankUp) and the remaining 50% for testing. The following document collections were used:

* Hulth 2003
* IEEE Explore
* Kaggle
* Twitter

## Hulth 2003

The original Hulth [1] collection consists of 2,000 abstracts with their corresponding title and keyphrases, and it has been used in several works as a benchmark for keyphrase extraction techniques. The abstracts belong to journal papers under the subjects of Computers and Control and Information Technology. The corpus is divided into three subsets: 1,000 abstracts for training, 500 for validation, and 500 for testing. In order to directly compare our results with those of other methods, we use the testing subset in our experiments. The collection originally contained controlled and uncontrolled keyphrases assigned by human annotators, of which we only use the uncontrolled set.

The validation set is also provided here.

## IEEE Explore

This collection was gathered from the IEEE Xplore digital library [2]. A web crawler was developed to crawl this source and extract abstract texts with their corresponding manually assigned keyphrases. A total of 417 abstracts belonging to scientific papers published in IEEE journals and conference proceedings were used for testing. The abstracts collected belong to 16 different subjects, ranging from aerospace engineering to signal processing.

## Kaggle

This collection was gathered from the Kaggle on-line data science competition platform [3]. It consists of 1,876 user questions on diverse topics from the Stack Exchange network. Each question has a set of tags given by the asker, which may be considered as the question's keyphrases.

## Twitter

This dataset consists of 1,314 English tweets from Twitter posted on April 2011 [4]. The tweets have been assigned keyphrases manually by human experts through the Mechanical Turk platform [5]. Each tweet was evaluated by three assigners, where each assigner had to choose between 1 and 4 keyphrases for each evaluated tweet; irrelevant tweets or those with no particular keyphrases were discarded. The final set of keyphrases selected for each tweet was made by selecting only those terms that had an agreement ratio of at least 2/3, that is, at least 2 of the 3 assigners had to have selected that term as a keyphrase.

# Data files

The four datasets are organized in two kinds of CSV files:
* texts: Contains the texts of each document and other supporting data
* keywords: Contains the keywords corresponding to each document

## Texts files

### File name format

collection_name_texts.csv

### Fields

* `document_id`: int, the ID of the document
* `category`: text, the category/domain of the text
* `original_text`: text, the original text of the document
* `stemmed_text`: text, the stemmed text of the document
* `word_count`: int, the number of words in the text
* `keyword_percentage`: the percentage of the keywords that actually appear in the text (stemmed)

## Keywords files

### File name format

collection_name_keywords.csv

### Fields

* `document_id`: int, the ID of the document (corresponding to a document in collection_name_texts.csv)
* `keyword`: text, a manually assigned keyword for the given document

# References

* [1] Anette Hulth. 2003. Improved automatic keyword extraction given more linguistic knowledge. Proceedings of the 2003 conference on Empirical methods in natural language processing, pages 216–223.
* [2] Institute of Electrical and Electronics Engineers. 2011. IEEE Xplore. http://ieeexplore.ieee.org/. [Online; accessed March-2011].
* [3] Kaggle. 2013. Kaggle. http://www.kaggle.com. [Online; accessed December-2013].
* [4] Twitter. 2011. Twitter. http://www.twitter.com. [Online; accessed April-2011].
* [5] Amazon. 2011. Amazon mechanical turk. http://www.mturk.com/. [Online; accessed August-2011].