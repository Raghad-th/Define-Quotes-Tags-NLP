Skip to content
Search or jump to…
Pull requests
Issues
Marketplace
Explore
 
@Raghad-th 
Madahus4
/
ARABIC-POEMS-USING-NLP
Public
Code
Issues
Pull requests
Actions
Projects
Wiki
Security
Insights
ARABIC-POEMS-USING-NLP/Arabic_Poems_report.md
@Madahus4
Madahus4 Update Arabic_Poems_report.md
Latest commit d4c560f on Nov 21
 History
 1 contributor
68 lines (57 sloc)  2.24 KB
   
# Abstract
The main focus of this project is develop an Arabic poems topic modeling to predict the correct phase of poems that can correctly classify the topic.

# Data Description
The datase that will be used in this project has been downloaded from [here]( https://hci-lab.github.io/LearningMetersPoems/).the total number of terms is **1,831,770** poetic terms. Each terms is labeled by its **meter**, the poet who wrote it, and the **age** which it was written in. There are **22 meters**, **3701 poets and 11 ages**: Pre-Islamic, Islamic, Umayyad, Mamluk, Abbasid, Ayyubid, Ottoman, Andalusian, era between Umayyad and Abbasid, Fatimid, and finally the modern age.  It is important to note that the terms diacritic states are not consistent. This means that a term can carry full, semi diacritics, or it can carry nothing.

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
    

    
    
    
© 2021 GitHub, Inc.
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
