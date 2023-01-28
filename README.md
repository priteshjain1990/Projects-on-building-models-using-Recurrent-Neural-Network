# Projects-on-building-models-using-Recurrent-Neural-Network
Projects - Stock Price Prediction, Spam Msg Classification, Forecasting Service Loads.

## Spam message classification
Spam Message Classification Using Recurrent Neural Network. 
First layer is Embedded layer where the embedded matrix is given as weights.
Second layer is LSTM, and the last is Dense later with softmax activation function to classify whether Spam or Ham. 
Glove is prebuilt embedded matrix used in project (downloaded from internet) which had 6B tokens with 50 features to build our own embedded matrix.

##  Stock Price Prediction
Stock Price Prediction of any arbitrary company (here in our example we considered Facebook). 
If the stocks prices are given for the entire previous year and we need to predict the price for next day.
Had use the lookback to create multiple sample dataset. If 'X' is the i/p sample and 'Y' is the lookback value, then we can create X-Y-1 samples dataset. Had used this technique to create the datasets. 
We build a keras Sequential model with SimpleRNN and Dense layers. 
ADAM was the optimizer used during compilation and 'mean squared error' is the loss function.
