# Restaurant Brands Clustering

## Intro
This repo is to cluster together restaurant brands based on their menu items being used in semantically similar contexts. 

## Datasets
csv file with only two columns: 

## Workflow
- read data with pandas
- food name embedding with sentence_transformers
- restaurant brand embedding using mean
- reduce the embedding dimensionality with PCA
- cluster the data with KNN
- visualize result with matplotlib

## Results
- This is the results of cluster restaurants into 10 clusters:
<img width="393" alt="pic" src="https://user-images.githubusercontent.com/30235642/177030660-f947b396-9778-49ff-a38d-0cbf2299b91f.png">

- Here is one example result:
```
Portillo's and Sujata are clustered into the same group.
[ Portillo's ] has food:  Tuna Salad Sandwich
[ Sujata ] has food:  Roti
It makes sense becuase Tuna Salad Sandwich is similar to Roti(a kind of bread).
```
