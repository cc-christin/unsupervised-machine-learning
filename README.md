# unsupervised-machine-learning
## Background
Predicting cryptocurrency clusters as a financial consultant in an advisory service team, for an investment banking client interested in starting a new cryptocurrency investment portfolio for their customers.

## Ask
* create a report of what cryptocurrencies are trending on the market
* determine whether the cryptocurrencies can be grouped to create classification systems for a new investment portfolio
* Give raw unlabeled data, process, fit, determine groupings, visualize,...

### Data Preparation
* read in crypto_data.csv using pandas obtained from [CryptoCompare](https://min-api.cryptocompare.com/data/all/coinlist).

* discarded non-traded cryptocurrencies
* removed in all rows with null values
* filtered mined cryptos
* convert all data to numerics
* standardize dataset

### t-sne
![T-SNE](https://github.com/cc-christin/unsupervised-machine-learning/blob/main/tsne.png)

### Cluster Analysis with k-Means
* created elbow plot to id best number of clusters
* use for loop to determine inertia for each k between 1 and 10
* elbow plot shows decline in cryptocurrencies without any specific clusterings

### elbow
![elbow](https://github.com/cc-christin/unsupervised-machine-learning/blob/main/Images/elbow.png)

### Recommendation
Based on currently available data, we would be apprehensive to recommend any cryptocurrencies for investment as definitive clusters could not be determined. The k-mean elbow curve shows a steady decline without any notable clusters. The t-sne on the other hand, has a clustering of unlabeled cyrptocurriences and a spaced out distirbution of others cryptocurrencies.
