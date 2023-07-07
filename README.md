# stockprediction
tesla stock price prediction on data from 2010 to 2020 using lstm


data has been taken from kaggle (https://www.kaggle.com/datasets/timoboz/tesla-stock-data-from-2010-to-2020?datasetId=500872)

Here,I used a Long Short Term Memory Network (LSTM) for building the model to predict the stock prices of Google.

LTSMs are a type of Recurrent Neural Network for learning long-term dependencies. It is commonly used for processing and predicting time-series data.LSTMs work in a three-step process.

1.The first step in LSTM is to decide which information to be omitted from the cell in that particular time step. It is decided with the help of a sigmoid function. It looks at the previous state (ht-1) and the current input xt and computes the function.

2.There are two functions in the second layer. The first is the sigmoid function, and the second is the tanh function. The sigmoid function decides which values to let through (0 or 1). The tanh function gives the weightage to the values passed, deciding their level of importance from -1 to 1.

3.The third step is to decide what will be the final output. First, you need to run a sigmoid layer which determines what parts of the cell state make it to the output. Then, you must put the cell state through the tanh function to push the values between -1 and 1 and multiply it by the output of the sigmoid gate

the modules used are:
pandas
numpy
matlabplotlib
tensorflow
sklearn
