# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
Step 1: Start

Step 2: Data Preparation: Load and explore customer data.

Step 3: Determine Optimal Clusters: Use the Elbow Method to find the best number of clusters.

Step 4: Apply K Means Clustering: Perform clustering on customer data.

Step 5: Visualize Segmented Customers: Plot clustered data to visualize customer segments.

Step 6: End

## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
import pandas as pd
import matplotlib.pyplot as plt
from sklearn.cluster import KMeans


data = {
    'CustomerID': [1,2,3,4,5,6,7,8,9,10],
    'Gender': ['Male','Female','Female','Male','Female','Male','Male','Female','Female','Male'],
    'Age': [19,21,20,23,31,22,35,30,25,28],
    'Annual Income (k$)': [15,16,17,18,19,20,21,22,23,24],
    'Spending Score (1-100)': [39,81,6,77,40,76,6,94,3,72]
}

df = pd.DataFrame(data)


X = df[['Annual Income (k$)', 'Spending Score (1-100)']]


kmeans = KMeans(n_clusters=3, init='k-means++', random_state=42)
df['Cluster'] = kmeans.fit_predict(X)  # Automatically fits and assigns clusters

plt.figure(figsize=(8,6))
for i in range(3):
    plt.scatter(X[df['Cluster']==i]['Annual Income (k$)'],
                X[df['Cluster']==i]['Spending Score (1-100)'],
                label=f'Cluster {i+1}')

# Plot centroids
plt.scatter(kmeans.cluster_centers_[:,0], kmeans.cluster_centers_[:,1],
            s=200, c='yellow', label='Centroids', marker='X')

plt.title('Customer Segmentation (K-Means)')
plt.xlabel('Annual Income (k$)')
plt.ylabel('Spending Score (1-100)')
plt.legend()
plt.show()


print(df)
Developed by: Vemareddygari Pallavi
RegisterNumber:  212225230293
*/
```

## Output:
<img width="951" height="657" alt="image" src="https://github.com/user-attachments/assets/eb1f7a49-6bef-4d86-834a-96fbe60703f4" />

<img width="1035" height="527" alt="image" src="https://github.com/user-attachments/assets/b933a9a4-6208-4310-a610-e59b255fc917" />


## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
