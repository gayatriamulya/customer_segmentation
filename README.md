# Customer Segmentation and Analysis
In this project, I have employed clustering, an unsupervised machine learning algorithm, to try to find hidden patterns in the spending patterns of different customers at a mall, which can be used to provide valuable insight into who and how the mall should focus its marketing efforts in order to increase its profits. 

![image](https://github.com/gayatriamulya/customer_segmentation/assets/138921379/cf007f4b-5484-446d-9625-6dc77773c4e4)

 (Fig 1)

There are 4 columns to take into account while performing the analysis – Gender, Age, Annual Income (k$), and Spending Score (1-100).


![image](https://github.com/gayatriamulya/customer_segmentation/assets/138921379/348db746-9de4-4bda-9403-a2ac97b23f15)
 (Fig 2)

We can see that the majority of customers are in the age group 30-40, the majority of customers have an annual income between $60k-$80k, and the majority of customers have a spending score of around 50. 





 ![image](https://github.com/gayatriamulya/customer_segmentation/assets/138921379/660b8d7b-26c7-453b-b888-7daaf7ae7d06)
(Fig 3)

 ![image](https://github.com/gayatriamulya/customer_segmentation/assets/138921379/b409a283-4190-4684-b4df-3703f547df36)
(Fig 4)
 ![image](https://github.com/gayatriamulya/customer_segmentation/assets/138921379/6d528305-dd98-431d-a891-493a7a71d1fd)
(Fig 5)

 ![image](https://github.com/gayatriamulya/customer_segmentation/assets/138921379/2d26149f-1489-4bd5-ad16-086144762a49)
 (Fig 6)   ![image](https://github.com/gayatriamulya/customer_segmentation/assets/138921379/97f30a78-b4aa-4683-baa5-363e6c1e8628)
(Fig 7--Means)                   
             
We can see that women make up the majority of the mall’s customers (56%), and have a higher average spending score compared to men. This means that the mall is doing a good job satisfying female customers, but needs to work on marketing and advertising targeted towards men.

 ![image](https://github.com/gayatriamulya/customer_segmentation/assets/138921379/d0a3b3ed-90fa-450b-913c-35c88b62676e)
(Fig 8)	 ![image](https://github.com/gayatriamulya/customer_segmentation/assets/138921379/f15af9d4-f637-4618-a179-a1e9292bd93c)
(Fig 9)

By looking at the correlation plot and the scatter plot of Spending Score vs. Age above (Fig 8 & Fig 9), we can deduce that as age increases, the number of customers with very high spending scores (i.e., above 60) decreases. This suggests that the mall needs to work on marketing and advertising, or other means in order to generate more profits from customers above the age of approximately 35-40. 


Now, we start with Clustering. 
![image](https://github.com/gayatriamulya/customer_segmentation/assets/138921379/d697a7e1-669b-43da-be27-613f6737472d)
 (Fig 10)
 
Using the elbow method, we find that the ideal number of clusters to separate customers by annual income is approximately 3 (low income, medium income, and high income).

![image](https://github.com/gayatriamulya/customer_segmentation/assets/138921379/23b211b5-1f81-4b3e-bd00-b19de8e3f76c)
 (Fig 11)	 ![image](https://github.com/gayatriamulya/customer_segmentation/assets/138921379/8143e6c1-958d-4dc3-bc4e-4cb5ae8da481)
(Fig 12-Means)

(Cluster 0—low income, cluster 1—medium income, cluster 2—high income)
We can see from Fig 11 that there are a large number of high income earners, however, according to Fig 12, their average spending score is the almost the same as customers of lower income levels. High income earners have more potential to spend, but they are currently not spending according to their potential, so the mall needs to work on marketing towards high income earners and focus on increasing profits from high income earners.

![image](https://github.com/gayatriamulya/customer_segmentation/assets/138921379/767101da-f4b7-47bb-89e9-65cfb83d4be4)
 (Fig 13)

Using the elbow method once again, this time for bivariate analysis, we find that the ideal number of clusters to divide the customer pool based on Annual Income and Spending Score is 5.
 ![image](https://github.com/gayatriamulya/customer_segmentation/assets/138921379/f5821bfa-c4e5-4914-aad7-1c004089f71f)
(Fig 14)

Plotting Annual Income vs. Spending Score, we observe there are 5 clusters of customers. Cluster 0—Medium income, Medium spending score.
Cluster 1 – Low income, high spending score
Cluster 2 - High income, High spending score
Cluster 3 – high income, low spending score
Cluster 4 – low income, low spending score

![image](https://github.com/gayatriamulya/customer_segmentation/assets/138921379/a057e7a0-f051-44d1-857c-4ae7ed16127e)
 (Fig 15)	
 ![image](https://github.com/gayatriamulya/customer_segmentation/assets/138921379/d5cacc33-411d-4e77-99f5-a26b0d79416a)
(Fig 16—Means)

Further, from Figure 15, we can see that the only cluster where there is a higher percentage of men than women is Cluster 3 – High income, low spending score. And we can see from Fig 16 that the lowest average spending score is in Cluster 3, even though the highest average income is also in Cluster 3.



## **Conclusions:**

Figs 14, 15, and 16 indicate that the mall should focus on increasing its profits from Cluster 3, i.e., high income earners with a low spending score. Their high income suggest that they have the potential to spend more, but are not spending it. We also know that there happen to be more men in Cluster 3 than women, and that the average age of customers in Cluster 3 is 41. So, the mall should make more efforts to market towards and increase its profits from high earning men in their 40s. 


