## Installation

Shell command:

`git clone https://github.com/andyc1997/collecting_analyzing_big_data.git`

`pip install -r requirements.txt`

---

## Description

1. Data are collected with [Collecting.ipynb](Collecting.ipynb) using *bs4.BeautifulSoup* and *requests*.

2. A initial data cleaning is performed to organize the data file in a structural way [Cleaning.ipynb](Cleaning.ipynb) using *pandas* and *numpy*.

3. Lemmatization, POS tagging and stopwords removal are applied to the cleaned data to tidy up the text for each comment [Tagging_and_lemmatization.ipynb](Tagging_and_lemmatization.ipynb). Here, we use *NLTK* for POS tagging and stopwords removal and *WordNet* for lemmatization.

4. Topic modeling and Text classification using *gensim* and *scikit-learn* framework. Both unigram and bigram are considered in topic modeling. For ordinal classification, we use [*mord*](https://pythonhosted.org/mord/) to fit ordianl logistic regression model with regularization. It is a library in python focusing on ordianl data. 

## Data source

Source webpage: [https://www.whatuni.com/](https://www.whatuni.com/) 

It is a webpage for students to review the universities in the U.K. Members can leave comments in text and give rating from 1 to 5. For this project, we consider Oxford, Edinburgh and Warwick based on my academic interests.
