# Abstract
The main focus of this project is predict a tags topic modeling to predict the correct tag of quote can correctly classify the topic.

# Design:
Using supervised and semi-supervised learning with Natural Learning Processing (NLP), throughout the project we will categorize the tag category based on the quote.So that when someone writes this quote it will give a quote similar to the quote's category.


# Data:
We have 2 dataset  the first one from Kaggel consist of 499,709 with 3 features and the second one web scraping from goodreads contain 83,618 with 3 features.
After pre-processing we decide to used data from kaggel because it is more useful, specifically the length of the quotes and topic modelling. The features consist of quotes, authers and category

# Algorithms
1. Exploratory Data Analysis was done to the dataset.
  - **Cleaning**
      - Checked for nulls values.
      -  Checked for duplicates and remove.
      -  Chose a sample of 10,000 rows.
      -  Romoved unneeded columns.
  - **Natrual Langauge Processing**
       - Remove harakat, tashkeel and tatweel
       - Remove extra spaces and punctuations
       - Remove numbers
       - Replace [آ إ أ] with [ا]
       - Replace [ؤ] with [و]
       - Replace repeated letter with single letter like [وو]  ,[ىى],[اا].
       - Vectorization.
       - Tokenization.
       - Stemming.
       - Remove Stop Word.
2. Topic Modeling
- Non-Negative Matrix Factorization (NMF).
- Latent Semantic Analysis (LSA).
- Latent Dirichlet Allocation (LDA).
- CorEx

3. Classification
- 7 classification models were built:
    - **XGBClassifier**
    - Gaussain Naive Bayes 
    - Support vector machines (SVMs)
    - Random Forest
    - Multinomial Naive Bayes
    - Decision Tree 
    - Logistic Regression

4. Clustering
- We calculates the inertia for 1 to 5 clusters.
- PCA to easily visualize clustering
- TSNE



## Tools:
* Software Platform :Jupyter Notebook
* Programming Language: Python
* Python Libraries:
  * Statistics libraries:
  * Sklearn
  * nltk
* Data manipulation libraries:
  * Pandas
  * Numpy
  * byArabic package
  * camel tool
* Visualization libraries
  * Matplotlib
  * Seaborn
* Storage libraries
  * Pickle

# Conclusion

CoreEx with Anchors the best in displaying topics.
