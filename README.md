# Cryptocurrencies
Module 18 - Unsupervised Machine Learning 

**Challenge file**: [crypto_clustering.ipynb file](https://github.com/GabrielaTuma/Cryptocurrencies/blob/c206f38f7ea20b15aa6f72168f420194902bbd15/crypto_clustering.ipynb) 


#### Deliverable 1

- [x] 1. All cryptocurrencies that are not being traded are removed
- [x] 2. The IsTrading column is dropped
- [x] 3. All the rows that have at least one null value are removed
- [x] 4. All the rows that do not have coins being mined are removed
- [x] 5. The CoinName column is dropped
<kbd>
  <img src="https://github.com/GabrielaTuma/Cryptocurrencies/blob/c206f38f7ea20b15aa6f72168f420194902bbd15/Images/1%20-%20df%20.png">
</kbd>  &nbsp;
</p>

- [x] 6. A new DataFrame is created that stores all cryptocurrency names from the CoinName column and retains the index from the crypto_df DataFrame

<kbd>
  <img src="https://github.com/GabrielaTuma/Cryptocurrencies/blob/c206f38f7ea20b15aa6f72168f420194902bbd15/Images/1%20-%20name_df.png">
</kbd>  &nbsp;
</p>

- [x] 7. The get_dummies() method is used to create variables for the text features, which are then stored in a new DataFrame
- [x] 8. The features from the X DataFrame have been standardized using the StandardScaler fit_transform() function

#### Deliverable 2

- [x] 1. The PCA algorithm reduces the dimensions of the X DataFrame down to three principal components
- [x] 2. The pcs_df DataFrame is created and has the following three columns, PC 1, PC 2, and PC 3, and has the index from the crypto_df DataFrame

<kbd>
  <img src="https://github.com/GabrielaTuma/Cryptocurrencies/blob/c206f38f7ea20b15aa6f72168f420194902bbd15/Images/2%20-%20pcs_df.png">
</kbd>  &nbsp;
</p>


#### Deliverable 3

- [x] 1. An elbow curve is created using hvPlot to find the best value for K


<kbd>
  <img src="https://github.com/GabrielaTuma/Cryptocurrencies/blob/c206f38f7ea20b15aa6f72168f420194902bbd15/Images/3%20-%20Elbow%20Curve.png">
</kbd>  &nbsp;
</p>

- [x] 2. Predictions are made on the K clusters of the cryptocurrencies’ data
- [x] 3. A new DataFrame is created with the same index as the crypto_df DataFrame and has the following columns: Algorithm, ProofType, TotalCoinsMined, TotalCoinSupply, PC 1, PC 2, PC 3, CoinName, and Class

<kbd>
  <img src="https://github.com/GabrielaTuma/Cryptocurrencies/blob/c206f38f7ea20b15aa6f72168f420194902bbd15/Images/3%20-%20clustered_df.png">
</kbd>  &nbsp;
</p>


#### Deliverable 4
- [x] 1. The clusters are plotted using a 3D scatter plot, and each data point shows the CoinName and Algorithm on hover

<kbd>
  <img src="https://github.com/GabrielaTuma/Cryptocurrencies/blob/c206f38f7ea20b15aa6f72168f420194902bbd15/Images/4%20-%203d_plot.png">
</kbd>  &nbsp;
</p>

- [x] 2. A table with tradable cryptocurrencies is created using the hvplot.table() function

<kbd>
  <img src="https://github.com/GabrielaTuma/Cryptocurrencies/blob/c206f38f7ea20b15aa6f72168f420194902bbd15/Images/4%20-%20hvplot_table.png">
</kbd>  &nbsp;
</p>

- [x] 3. The total number of tradable cryptocurrencies is printed
- [x] 4. A DataFrame is created that contains the clustered_df DataFrame index, the scaled data, and the CoinName and Class columns
- [x] 5. A hvplot scatter plot is created where the X-axis is "TotalCoinsMined", the Y-axis is "TotalCoinSupply", the data is ordered by "Class", and it shows the CoinName when you hover over the data point

<kbd>
  <img src="https://github.com/GabrielaTuma/Cryptocurrencies/blob/c206f38f7ea20b15aa6f72168f420194902bbd15/Images/4%20-%20scatter_plot.png">
</kbd>  &nbsp;
</p>


## Resources

- Software: Python 3.7.6, Visual Studio Code 1.58.1, Jupyter Notebook 6.3.0


