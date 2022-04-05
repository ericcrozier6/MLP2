Naive Bayes by Eric Crozier:

The naive bayes code performs classifications on datasets, of which label they belong to.

The code starts by creating the 3 functions MAP,MLE, and classify. From there in order to try 
save time, classify every word in the data set so we don't classify the same word twice. 
This is probably a naive way to do it, the code can take a decent amount of time to run.

Then we take each document and extract the classification for each word used to find the most 
likely label of the document. 

Then compare to the actual results of the documents (stored in the last row of the data set).

All of the words classifications are stored in a text file (words.txt), and the results of 
classifications done on documents are stored in classes.txt

This is not the best way to do things, but my code was too slow to risk having to rerun it 
more than necessary.

