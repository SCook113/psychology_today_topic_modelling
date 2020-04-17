# psychology_today_topic_modelling 

In this project I crawled articles from www.psychologytoday.com published between 2005 and this year and tried to determine the topics that are most written about / people are interested in.

For this I have written a script that crawls the website and stores published articles as well as some data about these articles (category/author/title etc.). After downloading the articles I uploaded them to https://community.cloud.databricks.com/ and did some analysis with pyspark. The notebook I used is also in this repository. After this I saved a subset of the data (the articles for the top category written about) for further analysis on my local machine. I then trained an lda model on the data and did some topic modelling.

The data that was crawled is not included in this repository.

Files and directories:

data/
All data used in this project. Not included in the repo.

model_lda/
The trained lda model.

crawling_data.ipynb
The notbook for crawling data from psychologytoday.

databricks_analysis.ipynb
The notebook in which analysis was made using pyspark.

investigating_topics_with_lda_model.ipynb
Here I train the model on a subset of the data.