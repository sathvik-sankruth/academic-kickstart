+++

title="Phase2 Classifier "

+++
**Phase 2**
Classifier: Multinomial Naïve Bayes Classifier<br>
Website Link : http://satsankruth.pythonanywhere.com/ <br>
Github Link:

A classifier is an algorithm that separates similar objects based on some features. For example, A video can be classified into music, autos & vehicles, comedy, gaming based on the category. However, what if we want to classify a new video? This can be done using very simple concept of probability, which is Naïve Bayes. Naïve Bayes is one of the popular classifiers when it comes to text classification. We can calculate the conditional probability of each term in the dataset’s vocabulary appear in each category.

**1. Preprocessing:** <br>
Because the data set has many repeated items with 40K rows, data set was modified so that it has only unique items which was reduced to 6K rows. 

![img](https://sathvik-sankruth.netlify.com/img/class1.PNG)

After saving the new data set, we convert to lowercase, perform stemming and eliminate stop words to construct a full vocabulary list.
 
**2. Processing:** <br>
Naïve Bayes classification is implemented using the formula.

$$ P(A \mid B) = \frac{P(B \mid A) \, P(A)}{P(B)} $$

Therefore, the mission is to construct a table to store the conditional probability for each term in the vocabulary with respect to each category.

![img](https://sathvik-sankruth.netlify.com/img/class2.PNG)

However, first, for each class c in the categories, the prior probability would be the number of documents in class c divided by the total number of documents.

P(c)=Number of documents in c/ Total Number of documents

Then the conditional probability can be calculated by the frequency of term t in document belong to class c.

To avoid sparseness that would lead conditional probabilities to be zero, we should apply smoothing into the calculation. To do this, we add 1 to all the term to avoid 0 on the numerator and add the number of unique terms to the denominator for normalization.
 
**3. Classification:** <br>
1)query is given for classification <br>
2) preprocess the query  Stemming, and eliminate Stop Words. <br>
3) A score will be given for each class using Naïve Bayes. <br>
4)The final step is to sort the score. <br>

![img](https://sathvik-sankruth.netlify.com/img/class3.PNG)

**4. Contribution:** <br>
To avoid  sparseness which leads probabilities to be zero, Applied Smoothing hyperparameter to 1. <br>

The Data set was split into Test data and Train data from sklearn.model_selection which ensures even distribution of the data. <br>

![img](https://sathvik-sankruth.netlify.com/img/class4.PNG)

Compared the Naïve Bayes classifier and SVM and found that Naive Bayes classifier works better for my data set. <br>

![img](https://sathvik-sankruth.netlify.com/img/class5.PNG)
 
Shows the percentages of classes. <br>
 
**5. Challenges faced:** 
Optimizing the algorithm was a bit challenging. <br>
The data set has many repeated items with 40K rows. Modified data set so that it has only unique items, Hence dataset was reduced to 6K rows.  <br>
 


**Reference:** <br>

* https://medium.com/@bedigunjit/simple-guide-to-text-classification-nlp-using-svm-and-naive-bayes-with-python-421db3a72d34

* https://towardsdatascience.com/naive-bayes-document-classification-in-python-e33ff50f937e

* https://nlp.stanford.edu/IR-book/html/htmledition/naive-bayes-text-classification-1.html

* https://nlp.stanford.edu/IR-book/pdf/13bayes.pdf

