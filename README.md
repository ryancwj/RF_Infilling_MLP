# RF_Infilling_MLP
Infilling Missing Rainfall Data with MLP Regressor

![output](https://user-images.githubusercontent.com/93307196/192239659-6c3b7c76-752a-47ed-a23b-d90f0fc879cd.png)

Often rainfall (precipitation) stations have missing values in the dataset. This is usually overcome by supplementing satelite rainfall data or data from multiple nearby rainfall stations.
This is considered as relaible when the nearby rainfall stations or satellite rainfall data strikes a high regression with the observed data.
Due to the nature of storms which varies between time and space, rainfall stations are usually poorly correlated to one another. 
Errors usually stem from either amplitude or phase differences which simple regressions are not able to detect.
But both satellite rainfall data and actual data from other stations usually share similiar seasonal trends and distribution patterns.

Hence, machine learning algorithms like Scikit-Learn in Python3 is used to simulate and fill in the missing data.
This script uses the Multi-Layer Perceptrons (MLP) regression method. 
Data used to train the MLP regressor includes a rainfall timeseries with moderate correlation (R^2 = 0.6) to the dataset in question and CHIRPS satellite rainfall data at the location of the rainfall station in question.
