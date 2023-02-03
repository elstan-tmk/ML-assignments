# ML-assignments

CA02: Spam eMail Detection using Naive Bayes Classification Algorithm<br>

# <b>Assignment Description</b> </b>

In this exercise we shall train the model with set of emails labelled as either from Spam or Not Spam. <br>
There are 702 emails equally divided into spam and non spam category.<br>
Next, we shall test the model on 260 emails. We shall ask model to predict the category <br>
of this emails and compare the accuracy with correct classification that we already know.<br>

# Instructions
1. Read the code and understand the logic of every line of the code<br>
2. Complete the code (there are missing areas of the code and it is mentioned in the<br>
commented cells), such that the code runs properly and produces the exact same
result as displayed at the end of the notebook.<br>
3. Comment the code thoroughly using “markdown” texts and comment lines so that
the logic of the code is easily understandable. <br>

# Cleaning and Preparing the data <br>
There are two folders test-mails and train-mails. The train-mails will be used to train the model.


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
<br>

First line is subject and the content starts from the third line.<br>
<br>
If you navigate to any of the train-mails or test-mails, you shall see file names in two patterns:<br>
number-numbermsg[number].txt : example 3-1msg1.txt (this are non spam
emails)ORspmsg[Number].txt : example spmsga162.txt (these files are of spam
emails).<br>
<br>
The very first step in text data mining task is to clean and prepare the data for a model.<br>
In cleaning we remove the non required words, expressions and symbols from text.
Consider a text: “Hi, this is Alice. Hope you are doing well and enjoying your vacation.”<br>
Here the words like is, this, are, and etc. don’t really contribute to the analysis. Such <br>
words are also called stop words. Hence in this exercise, we consider only most
frequent 3000 words of dictionary from email.<br>
After cleaning what we need from every email document, we should have some matrix
representation of the word frequency.<br>
