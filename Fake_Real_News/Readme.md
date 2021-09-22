# Fake and Real News

Utilizing the dataset provided by [Kaggle](https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset) I've developed 
a solution to classify fake and real news articiles. I have utilized this [reference](https://www.kaggle.com/rushinaik/mission-torch-1) 
as a source for developing the solution.

The solution can be broken down into three steps.
1. Data cleanup: remove stopwords, urls, twitter tags and non essential words
2. Vectorize : utilizing the TF-IDF vectorizaton from [sklearn](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html) a simple 
vector is developed for each input 
3. Model: A single Pytorch model with no *embeddings* and not as complex as *BERT* model is utilzed to classify the articles

After splitting the data into 70-30 split the result is currently at ** 98.2 % **.

The code for each of the three steps is provided in *Fake_Real_News.ipynb* 

