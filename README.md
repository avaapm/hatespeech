# Large-Scale Hate Speech Dataset
This repository contains the utilized dataset in the paper "Large-Scale Hate Speech Detection with Cross-Domain Transfer". This study mainly focuses hate speech detection in Turkish and English. In addition, domain transfer success between hate domains is also examined.

## Dataset

The dataset is composed of 200,000 tweets. Half of them is Turkish and other half is English. We also have domain information of the hate speech. These domains are Religion, Gender, Race, Politics, Sports. Each domain has 20,000 tweets in each respective language. 5 hate annotations of the tweet are also given. Since we followed Twitter's Terms and Conditions, publish tweet IDs not the tweet content directly. Explanations of the columns of the file are as follows:

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

Distibution of tweets in the dataset is as follows:

| Lang. | Domain | Hate | Offen. | Normal | Total |
|----------|----------|----------|----------|----------|----------|
| EN | Religion<br>Gender<br>Race<br>Politics<br>Sport | 1,427<br>1,313<br>1,541<br>1,610<br>1,434 | 5,221<br>6,431<br>3,846<br>6,018<br>5,624 | 13,352<br>12,256<br>14,613<br>12,372<br>12,942 | 20k<br>20k<br>20k<br>20k<br>20k
| TR | Religion<br>Gender<br>Race<br>Politics<br>Sport | 5,688<br>2,780<br>5,095<br>7,657<br>6,373 | 7,435<br>6,521<br>4,905<br>4,253<br>7,633 | 6,877<br>10,699<br>10,000<br>8,090<br>5,994 | 20k<br>20k<br>20k<br>20k<br>20k
