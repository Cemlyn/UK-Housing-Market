# UK-Housing-Market

Project looks into the possibility of using custom geographic clusters to use in a House Price index. Many house price indices use standard geographic regions within their hedonic regressions which are defined by the structure of the UK's regional governments. This raises the question whether geogrpahic clusters defined by analysis can result in a more accurate hedonic regression, and therefore a more accurate House Price Index.

Data has been sourced from the ONS "price paid" dataset which lists the price paid for all UK properties (excl. Northern Ireland and Scotland), from 1995 to the present. The figure below shows the median house price for a selection of UK postcode districts (e.g.  LL26, SW1, etc...) over the sample period.

![alt text](https://github.com/Cemlyn/UK-Housing-Market/blob/master/Median_price_smth.png)

Using Agglomerative clustering and defining the number of clusters to be k=10 the resulting geographic clusters are produced:

![alt text](https://github.com/Cemlyn/UK-Housing-Market/blob/master/Median_Clust_10.png)

Obviously results shown here would likely not be palatable to anyone trying to build an house price index. By including an "Adjacency matrix" which details whether or not two postcode district are adjacent to each, the geographic stucture of the UK can be considered during the clustering process. This results in much improved plot below:

![alt text](https://github.com/Cemlyn/UK-Housing-Market/blob/master/Agg_clust_10.png)
