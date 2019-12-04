+++

title="Phase1 Search "

+++

**Phase1**

A search feature which ranks the result based on the tf-idf scores.

 Website Link : http://satsankruth.pythonanywhere.com/
 
 Github Link : https://github.com/sathvik-sankruth/Term-project

**How to Deploy code :**<br>
 Create an account in pythonanywhere<br>
 Create a virtual environment and install python3, flask, nltk, numpy, pandas<br>
 Add the files<br>
 Go to the http link<br>

**How code works:**<br>
 Read data which is a csv file from pandas.
 
 Preprocess data to lower case. 
 
 Remove punctuations and apostrophe. 
 
 Remove stop words using nltk. 
 
 Stem the data using Porter Stemming. 
 
 Calculate term frequency. 
 
 Calculate Inverse Document Frequency. 
 
 Store tf-idf in a new pickle file which saves lot of time. 


 Query Words: <br>
  The query input is taken from the html page.

  Process the query convert it to lower case.

  Remove stop words from query.

  Rank the documents based on the similarity

  The top 20 results are displayed.

**Calculating TF-IDF:**

 Term Frequency(TF)= Number of times the word occures in document / Total Number of words in document

 Inverse Document Frequency(idf)= log( Total Number of documents / Number of documents with the keyword )

 TF_IDF=TF*IDF 


**Challenges faced:**
 The data set is huge which has around 40K rows. Takes a long time for more than 40 seconds to read the data set and perform calculations for each query. Hence Im reading the dataset at the beginning of the search function and precalculating the tf-idf scores, so that it's easy to get the search result once the page is loaded.

**Contributions:**
 Implemented stop words reduction and stemming while calculating tf-idf. 
 Added pickle to save the initial loading time. 


**References:**

 * https://github.com/williamscott701/Information-Retrieval/blob/master/2.%20TF-IDF%20Ranking%20-%20Cosine%20Similarity%2C%20Matching%20Score/TF-IDF.ipynb

 * https://www.geeksforgeeks.org/removing-stop-words-nltk-python/

 * https://help.pythonanywhere.com/pages/Flask/

 * https://www.youtube.com/watch?v=M-QRwEEZ9-8


<br><br>
[Phase 2 Classify](https://sathvik-sankruth.netlify.com/project/phase2classifier/)
[Phase 3 Image Caption Search](https://sathvik-sankruth.netlify.com/project/phase3imagecaption/)
<br><br>

