# Customer Segmentation and Analysis
In this project, I have employed clustering, an unsupervised machine learning algorithm, to try to find hidden patterns in the spending patterns of different customers at a mall, which can be used to provide valuable insight into who and how the mall should focus its marketing efforts in order to increase its profits. 

![alt text](https://github.com/gayatriamulya/customer_segmentation/blob/main/Images/Fig%201.png?raw=true)

 (Fig 1)

There are 4 columns to take into account while performing the analysis – Gender, Age, Annual Income (k$), and Spending Score (1-100).


![alt text](https://github.com/gayatriamulya/customer_segmentation/blob/main/Images/Fig%202.png?raw=true)
 (Fig 2)

We can see that the majority of customers are in the age group 30-40, the majority of customers have an annual income between $60k-$80k, and the majority of customers have a spending score of around 50. 





 ![alt text](https://github.com/gayatriamulya/customer_segmentation/blob/main/Images/Fig%203.png?raw=true) (Fig 3)



 ![at text](https://github.com/gayatriamulya/customer_segmentation/blob/main/Images/Fig%204.png?raw=true)
(Fig 4)
 ![alt text](https://github.com/gayatriamulya/customer_segmentation/blob/main/Images/Fig%205.png?raw=true)
(Fig 5)

 ![alt text](https://github.com/gayatriamulya/customer_segmentation/blob/main/Images/Fig%206.png?raw=true)
 (Fig 6)   ![alt text](https://github.com/gayatriamulya/customer_segmentation/blob/main/Images/Fig%207.png?raw=true)
(Fig 7--Means)                   
             
We can see that women make up the majority of the mall’s customers (56%), and have a higher average spending score compared to men. This means that the mall is doing a good job satisfying female customers, but needs to work on marketing and advertising targeted towards men.

 ![alt text](https://github.com/gayatriamulya/customer_segmentation/blob/main/Images/Fig%208.png?raw=true)
(Fig 8)	 ![alt text](https://github.com/gayatriamulya/customer_segmentation/blob/main/Images/Fig%209.png?raw=true)
(Fig 9)

By looking at the correlation plot and the scatter plot of Spending Score vs. Age above (Fig 8 & Fig 9), we can deduce that as age increases, the number of customers with very high spending scores (i.e., above 60) decreases. This suggests that the mall needs to work on marketing and advertising, or other means in order to generate more profits from customers above the age of approximately 35-40. 


Now, we start with Clustering. 

![alt text](https://github.com/gayatriamulya/customer_segmentation/blob/main/Images/Fig%2010.png?raw=true)
 (Fig 10)
 
Using the elbow method, we find that the ideal number of clusters to separate customers by annual income is approximately 3 (low income, medium income, and high income).

![alt text](https://github.com/gayatriamulya/customer_segmentation/blob/main/Images/Fig%2011.png?raw=true)
 (Fig 11)	 ![alt text](https://github.com/gayatriamulya/customer_segmentation/blob/main/Images/Fig%2012.png?raw=true)
(Fig 12-Means)

(Cluster 0—low income, cluster 1—medium income, cluster 2—high income)
We can see from Fig 11 that there are a large number of high income earners, however, according to Fig 12, their average spending score is the almost the same as customers of lower income levels. High income earners have more potential to spend, but they are currently not spending according to their potential, so the mall needs to work on marketing towards high income earners and focus on increasing profits from high income earners.

![alt text](https://github.com/gayatriamulya/customer_segmentation/blob/main/Images/Fig%2013.png?raw=true)
 (Fig 13)

Using the elbow method once again, this time for bivariate analysis, we find that the ideal number of clusters to divide the customer pool based on Annual Income and Spending Score is 5.
 ![alt text](https://github.com/gayatriamulya/customer_segmentation/blob/main/Images/Fig%2014.png?raw=true)
(Fig 14)

Plotting Annual Income vs. Spending Score, we observe there are 5 clusters of customers. Cluster 0—Medium income, Medium spending score.
Cluster 1 – Low income, high spending score
Cluster 2 - High income, High spending score
Cluster 3 – high income, low spending score
Cluster 4 – low income, low spending score

![alt text](https://github.com/gayatriamulya/customer_segmentation/blob/main/Images/Fig%2015.png?raw=true)
 (Fig 15)	
 ![alt text](https://github.com/gayatriamulya/customer_segmentation/blob/main/Images/Fig%2016.png?raw=true)
(Fig 16—Means)

Further, from Figure 15, we can see that the only cluster where there is a higher percentage of men than women is Cluster 3 – High income, low spending score. And we can see from Fig 16 that the lowest average spending score is in Cluster 3, even though the highest average income is also in Cluster 3.



## **Conclusion:**

Figs 14, 15, and 16 indicate that the mall should focus on increasing its profits from Cluster 3, i.e., high income earners with a low spending score. Their high income suggest that they have the potential to spend more, but are not spending it. We also know that there happen to be more men in Cluster 3 than women, and that the average age of customers in Cluster 3 is 41. So, the mall should make more efforts to market towards and increase its profits from high earning men in their 40s. 


