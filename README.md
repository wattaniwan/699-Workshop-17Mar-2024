## Workshop: 14 March 2024 

## Unsupervised models with K-means in BigQuery

### 1. Create Dataset  
- Dataset ID: DemoKmeans
- Location type: Multi-region + EU

### 2. Create, evaluate and save model to BigQuery
- Data: bigquery-public-data.london_bicycles
- using  bigframes.pandas and bigframes.ml.cluster
- Modify **01-CreateModelClustering-BigQuery.ipynb** 
- Create 9 models using Kmeans with k = 2, 3, 4, ... , 10 
- Save models into BigQuery 

 > ds-on-gcp-111111.DemoKmeans.modelKmeans2
 
 > ds-on-gcp-111111.DemoKmeans.modelKmeans3
 
 > ...
 
 > ds-on-gcp-111111.DemoKmeans.modelKmeans10

- Save results into BigQuery 

 > ds-on-gcp-111111.DemoKmeans.ResultStationKmeans2
 
 > ds-on-gcp-111111.DemoKmeans.ResultStationKmeans3
 
 > ...
 
 > ds-on-gcp-111111.DemoKmeans.ResultStationKmeans10



### 3. Report the comparison on the model performances

- Davies–Bouldin index 
- Mean squared distance

| Methods | Davies–Bouldin index | Mean squared distance |
|---------|----------------------|-----------------------|
| Kmean(k=2) | ... | ... |
| Kmean(k=3) | ... | ... |
| Kmean(k=4) | ... | ... |
| Kmean(k=5) | ... | ... |
| Kmean(k=6) | ... | ... |
| Kmean(k=7) | ... | ... |
| Kmean(k=8) | ... | ... |
| Kmean(k=9) | ... | ... |
| Kmean(k=10) | ... | ... |
