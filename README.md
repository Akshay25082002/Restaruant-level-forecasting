Restaurant-Level-Forecasting
1)Took the dataset from the Featured Prediction competition on Kaggle which was originally published by Recruit Holdings.

2)Did some sort of Data preprocessing, in order to proceed with the model training.

Time Series
1)By using the Dickey-Fuller test, found that data is not stationary.
2)Converted the dependent feature into stationary.
3)Approached the following classical time series models:
	.ARIMA - Manual way of finding the params ie) (p,d,q)
	.Auto ARIMA - Auto Grid search to find those params
	.SARIMAX - Used external regressors to improve the accuracy with the view of the season pattern
4)As these classical time series models fail to provide the expected range of accuracy, jumped to State-of-Art model to gain accuracy over it.
5)Approached the State-of-Art time series model which is proposed by Meta.
	.FbProphet
6)Approached Ensemble techniques:
	.Boosting - XGBoost, CatBoost
	.Cohorted Ensemble
Among the approached strategies, I felt Boosting gave reasonable accuracy because of the nature of how Boosting is made just by reducing the errors sequentially. What a kind of initution behind it right!!!
