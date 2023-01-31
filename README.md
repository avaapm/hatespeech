# Large-Scale Hate Speech Dataset
This repository contains the utilized dataset in the LREC 2022 paper "Large-Scale Hate Speech Detection with Cross-Domain Transfer". This study mainly focuses hate speech detection in Turkish and English. In addition, domain transfer success between hate domains is also examined.

There are two dataset versions. 

**Dataset v1:** The original dataset that includes **100k tweet per English and Turkish**, published in LREC 2022. The annotations with **more than 60% agreement** are included.

**Dataset v2:** A more reliable dataset version that includes **68,597 tweets for English and 60,310 for Turkish**. The annotations with **more than 80% agreement** are included.

## Dataset v2 (hate_speech_dataset_v2.csv)

We acknowledge that some annotations in the original dataset (v1) are controversial. Therefore, we publish a more reliable dataset version (v2) that includes only the tweets with more than 80% annotator agreement. The dataset v2 has 128,907 tweets. 60,310 of them are Turkish, and 68,597 are English. Explanations of the columns of the file are as follows:

| Column Name  | Description |
| ------------- | ------------- |
| TweetID | Twitter ID of the tweet |
| LangID | Language of the tweet 0-Turkish, 1-English |
| TopicID | Domain of the topic 0-Religion, 1-Gender, 2-Race, 3-Politics, 4-Sports |
| HateLabel | Final hate label decision 0-Normal, 1-Offensive, 2-Hate |

Distibution of tweets in the dataset is as follows:

| Lang. | Domain | Hate | Offensive | Normal | Total |
|----------|----------|----------|----------|----------|----------|
| EN | Religion<br>Gender<br>Race<br>Politics<br>Sport <br>  **Total**| 328<br>255<br>405<br>343<br>286 <br> **1,617 (2%)**| 2,369<br>3,043<br>1,631<br>2,972<br>2,814 <br> **12,829 (19%)** | 10,713<br>9,537<br>12,566<br>9,994<br>11,341 <br> **54,151 (79%)** | 13,410<br>12,835<br>14,602<br>13,309<br>14,441 <br> **68,597**
| TR | Religion<br>Gender<br>Race<br>Politics<br>Sport <br> **Total**| 2,281<br>970<br>1,897<br>3,657<br>4,016 <br> **12,821 (21%)**| 3,814<br>3,385<br>2,276<br>1,529<br>3,930 <br>  **14,934 (25%)** | 5,058<br>8,353<br>8,236<br>6,251<br>4,657 <br> **32,555 (54%)**| 11,153<br>12,708<br>12,409<br>11,437<br>12,603 <br> **60,310**

## Dataset labeler (hate_speech_dataset_v2_labeler.csv)
This file contains the individual annotations for each tweet. There are 20 labelers, and each tweet is annotated by 5 labelers.

| Column Name  | Description |
| ------------- | ------------- |
| TweetID | Twitter ID of the tweet |
| labeler_i | Annotation of the ith annotator 0-Normal, 1-Offensive, 2-Hate |


## Dataset v1 (hate_speech_dataset.csv)

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

| Lang. | Domain | Hate | Offensive | Normal | Total |
|----------|----------|----------|----------|----------|----------|
| EN | Religion<br>Gender<br>Race<br>Politics<br>Sport <br> **Total** | 1,427<br>1,313<br>1,541<br>1,610<br>1,434 <br> **7,325 (7%)** | 5,221<br>6,431<br>3,846<br>6,018<br>5,624<br> **27,140 (27%)** | 13,352<br>12,256<br>14,613<br>12,372<br>12,942 <br> **65,535 (66%)**| 20,000<br>20,000<br>20,000<br>20,000<br>20,000 <br> **100,000**
| TR | Religion<br>Gender<br>Race<br>Politics<br>Sport <br> **Total**| 5,688<br>2,780<br>5,095<br>7,657<br>6,373<br> **27,593 (28%)** | 7,435<br>6,521<br>4,905<br>4,253<br>7,633<br> **30,747 (31%)**| 6,877<br>10,699<br>10,000<br>8,090<br>5,994<br> **41,660 (41%)**| 20,000<br>20,000<br>20,000<br>20,000<br>20,000 <br> **100,000**

## Citation
If you make use of this dataset, please cite following paper.

```bibtex
@InProceedings{toraman2022large,
  author    = {Toraman, Cagri  and  \c{S}ahinu\c{c}, Furkan and Yilmaz, Eyup Halit},
  title     = {Large-Scale Hate Speech Detection with Cross-Domain Transfer},
  booktitle = {Proceedings of the Language Resources and Evaluation Conference},
  month     = {June},
  year      = {2022},
  address   = {Marseille, France},
  publisher = {European Language Resources Association},
  pages     = {2215--2225},
  url       = {https://aclanthology.org/2022.lrec-1.238}
}

```
