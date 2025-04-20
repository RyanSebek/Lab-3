# Lab-3
MGT 665 - Lab 

# Health Clusters
## Abstract
The goal of this project was to train an AI model in predicting when someone might need a health intervention by using clustering. The models selected in this experiment were K means clustering and hierarchical clustering. 

## Introduction
Given the health status of 200 patients, I wanted to create a model that would help identify idividuals that are in need of a health intervention.

## Related Work
I used two studies to help guide this study. The first one by Ryan Holbrook, provided an excellent example of how to apply principle component analysis to a data set to make it more one dimensional. The second study by Gireesh Sundaram provided an complete guide to applying K means clustering.

## Methodology
In order to complete this task, I set out first preparing the data. Fortunately, not much preparation was needed for this dataset. The nextstep was EDA. For this I made a correlation matrix to determine if there were any variables that correlated well together. In the data set provided, all the variables really did not correlate well together, so I graphed the pairs. I know BMI is a very strong indicator of someones overall health, so I set this as the y variable and made all the other the x variables. I first did K means clustering and that returned a silhouette score of 0.201. I then did hierarchical clustering and that returned a score of 0.348. 

Once the original scores were obtained, I applied PCA analysis to see if it would improve the accuracy of the model. When applied to the K Means model, the score jumped from 0.201 to 0.428. On the other hand the hierarchical clustering slightly decreased to 0.334 from 0.348. 

## Results
The model that best predicted whether a intervention was needed or not was the PCA K means model. This model had a silhouette score of 0.428 which means that the average distance between the clusters was not that large. This model is pretty accurate for the data provided. 

## Discussion
Looking back at the model. I see some areas that could have been improved upon. While the models did do better than anticipated, especially with the limited correlation, I would try other models to make sure that the best one was selected. 

## References
Gireeshs. (2020, September 9). Complete Guide to Clustering Techniques. Kaggle. https://www.kaggle.com/code/gireeshs/complete-guide-to-clustering-techniques 
Ryanholbrook. (2023, April 20). Principal component analysis. Kaggle. https://www.kaggle.com/code/ryanholbrook/principal-component-analysis 
