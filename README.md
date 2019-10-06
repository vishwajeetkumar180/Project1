# Project1

Annual car sales  prediction using ARIMA Model:-

First import the essential libraries which are used in this project like numpy,matplotlib,pandas,sklearn etc.then
upload the datset of sales_car by using pandas in this datset two coloumns are there Month and sales,first we make month as index 
and by using date parser we put the date in every datapoints initially date is not there in dataset.

After that i plot the our datset by using plot function then i found that our data is looks like trend or we can say that dataset is not stationary, Then we first detrending the dataset by differencing ,it is also called as integrating of order 1 if we apply one time differencing then we plot acf,pacf plot.


After this we break our datset into two parts ie train dataset and test dataset
First I predict using Ar model after that arima i have used in the stasmodel there is tsa function in which armodel,arimamodel libraries are present then we import statsmodel.tsa.arima_model import ARIMA. We pass the train_data into the ARIMA model along with (p,d,q),where p is order of AR model,d is integrating order and q is order of MA model after that we apply the fit function for Fits ARIMA(p,d,q) model by exact maximum likelihood, after that i use forecast function and pass the parameter as number of steps to forecast then we plot the test_data and the forecasted data is likely same.
