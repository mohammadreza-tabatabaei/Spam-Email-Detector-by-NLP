# Requirements:
### 1.Numpy 
### 2.pandas 
### 3.seaborn 
### 4.nltk 
### 5.sklearn 

# Dataset:
I used spam_or_not_spam dataset which is available on kaggle. The csv file contains 5172 rows, each row for each email. There are 3002 columns. The first column indicates Email name. The name has been set with numbers and not recipients' name to protect privacy. The last column has the labels for prediction : 1 for spam, 0 for not spam. The remaining 3000 columns are the 3000 most common words in all the emails, after excluding the non-alphabetical characters/words. For each row, the count of each word(column) in that email(row) is stored in the respective cells. Thus, information regarding all 5172 emails are stored in a compact dataframe rather than as separate text files.

# Recognition Phase: 
At first, I deleted all the empty emails. Then, I removed all the stopwords using the NLTK library, and the roots of the words in the emails were obtained using the Lematization technique. Then spam emails were detected by different classifiers including SVC,RandomForest, LogisticRegression and MultinomialNB.
