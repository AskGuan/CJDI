# CJDI
CJDI:A Fine-Grained Chinese dataset for Jargon Detection and Interpretation

## 1. Content
We propose CJDI, a fine-grained Chinese dataset for Jargon Detection and Interpretation. CJDI consists of 90,852 messages containing 537 jargon words and a tree-structured jargon taxonomy comprising 10 jargon categories.

## 2. Quality
Our research follows AAAI ethical rules, and the data set does not contain user-profiles and sensitive information. We only collected the text content of Danmaku, and all raw data came from public data. The data set is easy to access, and the jargon taxonomy provided in this paper can support many levels of granularity, which enables our data set to adapt to different tasks.

## 3. Structure
This data set consists of two parts. The "raw" directory is the original data collected, which contains all the information of the Danmaku message (such as video number, the sending time of the Danmaku, and the content of the message). The "dataset" directory is created for jargon detection and interpretation tasks, internally divided into two directories. "Task1-training-test set" is the data set for the jargon detection task. The "annotation" directory provides jargon-related terms generated by user evaluation in the jargon interpretation task. The training data is saved in CSV format with three fields: Danmaku message, jargon word and jargon category.

## 4. Potential uses of the dataset
This dataset collects a large number of jargon from Chinese online communities, and annotates a variety of granularity of jargon types. Provides a large data set for jargon detection and jargon interpretation tasks.

## 5. Methodology employed for data collection
This data sampling covered all sub-communities of Bilibili. We selected the top 100 popular videos from each sub-community and finally got 3063 popular videos to collect Danmaku messages. We used python worm to crawl the Danmaku XML files and used the XML parser to extract the content.
