# Credit-Card-Customer-Segmentation

**Business Problem**<br><br>
Banks constantly need to customize their experience for their customers to remain competitive in the banking sector. Every year, banks are creating customized credit cards to fit the varying lifestyles of their customer base and personalize marketing strategies to broaden their target market. Knowing the specific characteristics of a bank’s customer base has become a critical piece to a bank’s vitality. This project aims to utilize clustering analysis to segment credit card users for companies. It could help companies offer customized credit card services for clients which increases their profitability.

**Dataset**<br><br>
Our dataset consists of 8950 rows and 18 columns. Each row represents an individual credit card customer and the columns are mostly credit card usage variables. Excluding the column representing customer id, the columns are all numeric. Among those numeric columns, we have 14 float variables and 3 integer variables. We confirmed our dataset has only two columns with NULL values; credit_limit and minimum_payments. We used median to fill in the 1 missing column from credit_limit and the 313 missing values from the minimum_payments column. We decided to use median after acknowledging the mean for the minimum_payment value is higher than over 75% of the dataset. This mean value then is skewed due to the outliers in the column and could be more disruptive than helpful. For these reasons, we’ll use the value that occurs in the middle of the data. We also scaled the data to ensure comparisons between variables exist on the same scale. 

**Method**<br><br>
1. Exploratory Data Analysis
2. Hierarchical Clustering and K-Mean Clustering
> * Used a dendrogram to visualize the hierarchical relationship
> * Recorded the inertia and the average silhouette score for different cluster sizes before conducting K-Means clustering
> * Used Principal Component Analysis (PCA) to reduce the column dimensions since we noticed highly correlated features in our Exploratory Data Analysis (EDA)
> * Examined the customer distribution for each cluster result we obtained from previous step
3. Conclusions and Recommendations

**Conclusion and Recommendation**<br><br>
We grouped all customers into seven categories, discovered characterisitics among each of them, and provided personalized suggestions. Cluster 2 and 3 possess high purchasing power. The ability of consuming in cluster 2 is higher than cluster 3. For these two clusters, the bank should encourage them to use more credit cards and offer more cash backs and discounts for credit card payment. Cluster 1, 5, 6 are defined as heavy cash advance user, with cluster 6 the heaviest. We recommend to look for what motivates these three clusters to use cash advance. If they use cash advance due to cash shortage, the bank should consider reduce credit limit, but if tight budget is not the case, the bank could advertise more cash advance service. Lastly, cluster 0 and 4 are customers with lower purchasing power. Since these two groups are not sticked to certain services, we suggest the bank remain usual marketing strategy.


