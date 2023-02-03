# ML-assignments

## CA02: Spam eMail Detection using Naive Bayes Classification Algorithm
This exercise will train the model with set of emails labelled as either from Spam or Not Spam. <br>
There are 702 emails equally divided into spam and non spam category. <br>
Next, the model will be tested on 260 emails. The category of this emails is going to be predict <br>
by the moedl and compare the accuracy with the correct classification. 
<br><br>
###Some Code Explanation
Cleaning and Preparing the data <br>
We have two folders test-mails and train-mails. We will use train-mails to train the
model. The sample email data set looks like: <br>

<br><br><br>
First line is subject and the content starts from the third line. <br>
If you navigate to any of the train-mails or test-mails, you shall see file names in two
patterns: <br><br>
number-numbermsg[number].txt : example 3-1msg1.txt (this are non spam
emails)ORspmsg[Number].txt : example spmsga162.txt (these files are of spam
emails). 
<br><br>
The very first step in text data mining task is to clean and prepare the data for a model. <br>
In cleaning we remove the non required words, expressions and symbols from text. <br>
Consider a text: “Hi, this is Alice. Hope you are doing well and enjoying your vacation.” <br>
Here the words like is, this, are, and etc. don’t really contribute to the analysis. Such <br>
words are also called stop words. Hence in this exercise, we consider only most
frequent 3000 words of dictionary from email. <br>
After cleaning what we need from every email document, we should have some matrix
representation of the word frequency.
