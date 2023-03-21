# Predictive-Maintenance
Objective :

My goal was to implement the two of the Predictive Maintenance Machine Learning
Techniques Technique 
1 - Regression Models to predict the remaining useful life (RUL) and Technique 
2 – Classification Model to Predict Failure Within a Pre-Decided Time Frame.

Dataset:
In my application I have used the Turbofan Jet Engine Data Set from NASA.

Description:
Prognostics and health management is an important topic in industry for predicting state
of assets to avoid downtime and failures. This data set is the Kaggle version of the very well
known public data set for asset degradation modeling from NASA. It includes Run-to-Failure
simulated data from turbo fan jet engines.
Engine degradation simulation was carried out using C-MAPSS. Four different were sets
simulated under different combinations of operational conditions and fault modes. Records
several sensor channels to characterize fault evolution. The Prognostics CoE at NASA Ames
provided the data set.

Prediction Goal:
In this dataset the goal is to predict the remaining useful life (RUL) of each engine in the
test dataset. RUL is equivalent of number of flights remained for the engine after the last
datapoint in the test dataset
Experimental Scenario
Data sets consists of multiple multivariate time series. Each data set is further divided
into training and test subsets. Each time series is from a different engine i.e., the data can be
considered to be from a fleet of engines of the same type. Each engine starts with different
degrees of initial wear and manufacturing variation which is unknown to the user. This wear and
variation is considered normal, i.e., it is not considered a fault condition. There are three
operational settings that have a substantial effect on engine performance. These settings are also
included in the data. The data is contaminated with sensor noise.
The engine is operating normally at the start of each time series, and develops a fault at
some point during the series. In the training set, the fault grows in magnitude until system
failure. In the test set, the time series ends some time prior to system failure. The objective of the
competition is to predict the number of remaining operational cycles before failure in the test set,
i.e., the number of operational cycles after the last cycle that the engine will continue to operate.
Also provided a vector of true Remaining Useful Life (RUL) values for the test data.
The data are provided as a zip-compressed text file with 26 columns of numbers,
separated by spaces. Each row is a snapshot of data taken during a single operational cycle, each
column is a different variable. The columns correspond to:
1) unit number
2) time, in cycles
3) operational setting 1
4) operational setting 2
5) operational setting 3
6) sensor measurement 1
7) sensor measurement 2
…
26) sensor measurement 26
