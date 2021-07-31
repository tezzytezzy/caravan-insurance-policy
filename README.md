# Caravan Insurance Policy

## Synopsis

Distinct classification models (Random Forest, Decision Tree, Ada Boost, and Gradient Boost) are applied and tested. This project starts with the standard training-and-validation set sampling ratio of 80:20. Cross-validation, out of bag scores (for well-randomized training and validation split), and grid search (for hyperparameter tuning) are deployed to reduce bias and error and make a generalized model, as samples are not time-sensitive (i.e., not time-series). While confusion matrix helps to assess granular improvement in the models, unpredictive features were eliminated through ranking of feature importance, correlation, and dendrogram.

## Data Set Information

Information about customers consists of 86 variables and includes product usage data and socio-demographic data derived from zip area codes. The data was supplied by the Dutch data mining company Sentient Machine Research and is based on a real world business problem. The training set contains over 5000 descriptions of customers, including the information of whether or not they have a caravan insurance policy. A test set contains 4000 customers of whom only the organisers know if they have a caravan insurance policy.

The data dictionary (DICTIONARY.txt) describes the variables used and their values.

Note: All the variables starting with M are zipcode variables. They give information on the distribution of that variable, e.g. Rented house, in the zipcode area of the customer.

One instance per line with tab delimited fields.

TICDATA2000.txt: Dataset to train and validate prediction models and build a description (5822 customer records). Each record consists of 86 attributes, containing sociodemographic data (attribute 1-43) and product ownership (attributes 44-86).The sociodemographic data is derived from zip codes. All customers living in areas with the same zip code have the same sociodemographic attributes. Attribute 86, "CARAVAN:Number of mobile home policies", is the target variable.

TICEVAL2000.txt: Dataset for predictions (4000 customer records). It has the same format as TICDATA2000.txt, only the target is missing. Participants are supposed to return the list of predicted targets only. All datasets are in tab delimited format. The meaning of the attributes and attribute values is given below.

TICTGTS2000.txt Targets for the evaluation set. 

## Reference
[Insurance Company Benchmark (COIL 2000) Data Set](https://archive.ics.uci.edu/ml/datasets/Insurance+Company+Benchmark+%28COIL+2000%29)
