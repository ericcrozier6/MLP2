Logistic Regression Read Me by Cody Crane

This program and read me assumes that you are running everything in jupyter notebook and that you have the testing.npz and training.npz files downloaded and in the same directory as this program as the program references both of them.

Since we should be working in jupyter notebook I will refer to sections of code by their cell as starting from cell one(1) at the top of the file.

This readme is a general overview if you would like or need more information refer to the comments in the program file

Cell #1: This cell imports the necessary librarys that we use throughout

Cell #2: This cell loads in and processes the training.npz and testing.npz files that contain our data for this project

Cell #3: This cell defines the getProbabilitys method that calculates the probabilites for a given set of examples and a given weight function

Cell #4: This cell defines the classify method that reads in a weight function from a file based on the given parameters and classifies the given data set, either the testing or training data set, with that weight function, it then formats and outputs the predictions to a csv file named according to the hyperparameters provided

Cell #5: This cell defines the updateWeights function that is used in the train function to update the weight matrix 

Cell #6: This cell defines the train function that trains a weight matrix based with the training data and the supplied hyperparameters

Cell #7: This cell provides some information on using the different functions appart from one another and how to make sure they work together

Cell #8: This cell defines the logisticRegression function that runs through the entire process, it trains a weight matrix using the given hyperparameters and then classifies the given dataset, for this example either 'training' or 'testing'.

If you would like to simply test our code over the testing set simply call
logisticRegression('testing', 0.01, 0.01, 10000)
this will train a weight function over ten thousand iterations with eta=0.01 and lambda 0.01
it will save that weight function to the file class_function_eta0.01_lmdb0.01_iter10000.csv
it will then use that weight function to classify the testing set and output its predictions to the file
TESTINGpredictions_eta0.01_lmdb0.01_iter10000.csv
this file is what we upload to kaggle for our submission