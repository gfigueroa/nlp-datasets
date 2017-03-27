# Text corpora for keyword extraction
===============================================================================

## Description of the collections

These text corpora are composed of research paper abstracts from different scientific journals, spanning a wide variety of domains.
For collections 2, 3, 4, and 6, each abstract text includes its manually-assigned keywords.
Collections 1 and 5 have different formats.
Be aware that the files use UNIX new line characters.
The texts can be used for the testing, training and validation of keyword extraction methods.

The following document collections are available:

1. Hulth 2003
2. IEEE Explore
3. Journal of Applied Physics
4. Journal of Psychiatric Practice
5. Twitter
6. VLDB Journal

### Hulth 2003

The original Hulth [1] collection consists of 2,000 abstracts with their corresponding title and keyphrases, and it has been used in several works as a benchmark for keyphrase extraction techniques. The abstracts belong to journal papers under the subjects of Computers and Control and Information Technology. The corpus is divided into three subsets: 1,000 abstracts for training, 500 for validation, and 500 for testing. The collection contains controlled and uncontrolled keyphrases assigned by human annotators, of which we only use the uncontrolled set. Please read the README.MD file provided for the Hulth 2003 corpus for more information.

### IEEE Explore

This collection was gathered from the IEEE Xplore digital library [2]. A web crawler was developed to crawl this source and extract abstract texts with their corresponding manually assigned keyphrases.
The IEEE Explore corpus has been further grouped into categories, including Aerospace Engineering, Bioengineering, Communications, etc.

### Journal of Applied Physics

This collection was crawled from the Journal of Applied Physics [3].

### Journal of Psychiatric Practice

This collection was crawled from the Journal of Psychiatric Practice [4].

### Twitter

The Twitter dataset consists of English tweets from Twitter posted on April 2011. 
The tweets have been assigned keyphrases by humans through the Amazon Mechanical Turk platform. 
Each tweet was evaluated by three assigners, where each assigner had to choose between 1 and 4 keyphrases for each evaluated tweet.
The final set of keyphrases selected for each tweet was made by selecting only those terms that had an agreement ratio of at least 2/3.

### VLDB Journal

This collection was crawled from the Very Large Databases Journal [5].

## Data files

The datasets, with the exception of Hulth 2003 and Twitter, contain one file for each abstract. Each file contains the abstract text and the keywords that were manually assigned by the author.

## Acknowledgment
These datasets are free for research use.
If you find them useful or use them in your research, please acknowledge my git repository!

## References

* [1] Anette Hulth. 2003. Improved automatic keyword extraction given more linguistic knowledge. Proceedings of the 2003 conference on Empirical methods in natural language processing, pages 216–223.
* [2] Institute of Electrical and Electronics Engineers. 2011. IEEE Xplore. http://ieeexplore.ieee.org/. [Online; accessed March-2011].
* [3] American Institute of Physics. 2011. Journal of Applied Physics. http://jap.aip.org/. [Online; accessed March-2011].
* [4] Lippincott Williams & Wilkings. 2011. Journal of Psychiatric Practice. http://journals.lww.com/practicalpsychiatry/pages/default.aspx/. [Online; accessed March-2011].
* [5] Very Large Databases Endowment Inc. 2011. Very Large Databases Journal. http://www.vldb.org/. [Online; accessed March-2011].