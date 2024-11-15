# Context-Aware Attention-Based Model for Enhanced Long term Traffic Prediction on Non-Graph-Structured Data

This is the tensorflow implementation of Context-Aware Attention-Based Model for Enhanced Long term Traffic Prediction on Non-Graph-Structured Data paper.
* You can access the dataset in the Datasets folder.
* You can see the implementation of the proposed model for each of the four data sets in different time resolutions in the folder specific to that data set.

## Proposed method
The proposed model consists of three main components: 
1. one-dimensional convolutional layer: to capture local dependencies between the feature vectors
2. a gated recurrent unit (GRU): to extract temporal dependencies in the data 
3. soft-attention layer: to better extract meaningful temporal patterns and long-term dependencies among the data

## Data
a dataset was collected by <a href="https://www.sciencedirect.com/science/article/pii/S0952197623002257">Long term traffic flow forecasting using a hybrid CNN-BiLSTM model</a> paper.
This dataset includes data from four traffic stations located in Madrid.
1.  Paseo de la Castellana (P/Castellana) is a major street in the city center, providing data in the north-tosouth direction.
2.  Calle Arturo Soria(C/Arturo Soria) is a long street in the east of the city, serving the north-to-south route of Madrid.
3. Paseo de Santa María de la Cabeza (P/Sta María) is a key route connecting the city center to the south
4. Gran Vía (C/Gran Vía) is a central shopping and tourist street, providing data in the west-to-east direction.

The variables included in these four datasets are as follows: 
* day type (holiday, weekday, or weekend)
* average daily temperature
* minimum daily temperature
* maximum daily temperature
* daily rainfall
* the number of vehicles on adjacent streets (for each main street, two adjacent streets were considered)
* the number of vehicles on the target street..



## Results
In the table below, it can be seen that the proposed model has been able to improve the evaluation criteria of RMSE, MAE, Accuracy compared to the basic models.


![alt text](https://github.com/majidhosseini87/Context-Aware-Attention-Based-Model-for-Enhanced-Long-term-Traffic-Prediction/blob/main/Figures/Experimental%20Results.png)
