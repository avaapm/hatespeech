# Large-Scale Hate Speech Dataset
This repository contains the utilized dataset in the paper "Large-Scale Hate Speech Detection with Cross-Domain Transfer". This study mainly focuses hate speech detection in Turkish and English. In addition, domain transfer success between hate domains is also examined.

## Dataset

The dataset is composed of 200,000 tweets. Half of them is Turkish and other half is English. We also have domain information of the hate speech. These domains are Religion, Gender, Race, Politics, Sports. Each domain has 20,000 tweets in each respective language. 5 hate annotations of the tweet are also given. Explanations of the columns of the file are as follows:

| Column Name  | Description |
| ------------- | ------------- |
| TweetID | Twitter ID of the tweet |
| LangID | Language of the tweet 0-Turkish, 1-English |
| TopicID | Domain of the topic 0-Religion, 1-Gender, 2-Race, 3-Politics, 4-Sports |
| Label_1 | Annotation of the first annotator 0-Normal, 1-Offensive, 2-Hate |
| Label_2 | Annotation of the second annotator 0-Normal, 1-Offensive, 2-Hate |
| Label_3 | Annotation of the third annotator 0-Normal, 1-Offensive, 2-Hate |
| Label_4 | Annotation of the fourth annotator 0-Normal, 1-Offensive, 2-Hate |
| Label_5 | Annotation of the fifth annotator 0-Normal, 1-Offensive, 2-Hate |
| HateLabel | Final hate label decision 0-Normal, 1-Offensive, 2-Hate |
