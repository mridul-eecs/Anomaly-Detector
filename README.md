# Anomaly-Detector

### Description: Our objective is to dedtect anomaly in a generator using vibration sensors

### Dataset: Dataset used for this case study is from Case Western Reserve University open bearings dataset.
http://csegroups.case.edu/sites/default/files/bearingdatacenter/files/Datafiles



### Excution steps:
- Downloaded dataset which in Matlab format into our data folder
- Read Matlab files using Scipy.io library as a python dictionary and transformed it into a dataframe and saved into a CSV file for further machine learning.
- Loaded dataframe and created an Autoencoder using LSTM cells.
- Unsupervised learning using autoencoders on keras framework.
- Autoencoder accuracy score is used as a threshold to label signals between fair and disturbed.
- Again this labelled dataset from our autoencoder is used for further machine learning.
- Feature engineering on the signals to convert them into frequency domains using FFT.
- Feature engineered dataset fed into simple feed forward network to predict Anomaly.
- Finally Anamoly detector is ready with an accuray of 96%.


