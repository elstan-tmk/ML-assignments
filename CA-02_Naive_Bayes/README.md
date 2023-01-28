# ML-assignments

## CA02: Spam eMail Detection using Naive Bayes Classification Algorithm
This exercise will train the model with set of emails labelled as either from Spam or Not Spam. \
There are 702 emails equally divided into spam and non spam category. \
Next, the model will be tested on 260 emails. The category of this emails is going to be predict \
by the moedl and compare the accuracy with the correct classification. 

###Some Code Explanation
Cleaning and Preparing the data \
We have two folders test-mails and train-mails. We will use train-mails to train the
model. The sample email data set looks like: \
Subject: re : 2 . 882 s - > np np> deat : sun , 15 dec 91 2 : 25 : 2 est > : michael <
mmorse @ vm1 . yorku . ca > > subject : re : 2 . 864 query
> > wlodek zadrozny ask " anything interest " > construction " s > np np " . . . second ,
> much relate : consider construction form > discuss list late reduplication ? > logical
sense " john mcnamara name " tautologous thus , > level , indistinguishable " , , here ? "
. ' john mcnamara name ' tautologous support those logic-base semantics irrelevant natural
language . sense tautologous ? supplies value attribute follow attribute value . fact
value name-attribute relevant entity ' chaim shmendrik ' , ' john mcnamara name ' false .
tautology , . ( reduplication , either . )
<br>
First line is subject and the content starts from the third line. \
If you navigate to any of the train-mails or test-mails, you shall see file names in two
patterns: \
number-numbermsg[number].txt : example 3-1msg1.txt (this are non spam
emails)ORspmsg[Number].txt : example spmsga162.txt (these files are of spam
emails). 
<br>
The very first step in text data mining task is to clean and prepare the data for a model. \
In cleaning we remove the non required words, expressions and symbols from text. \
Consider a text: “Hi, this is Alice. Hope you are doing well and enjoying your vacation.” \
Here the words like is, this, are, and etc. don’t really contribute to the analysis. Such \
words are also called stop words. Hence in this exercise, we consider only most
frequent 3000 words of dictionary from email. \
After cleaning what we need from every email document, we should have some matrix
representation of the word frequency.
