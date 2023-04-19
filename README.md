# Cryptocurrency-Machine-Learning-

Elbow Analysis with K-means using the Original Scaled Data and PCA Data:
- Create a list with the number of k values from 1 to 11.
- Create an empty list to store the inertia values.
- Create a for loop to compute the inertia with each possible value of k.
- Create a dictionary with the data to plot the elbow curve.
- Plot a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.

Cluster Analysis with K-means Using the Original Scaled Data and PCA Data:
- Initialize the K-means model with the best value for k.
- Fit the K-means model using the original scaled DataFrame.
- Predict the clusters to group the cryptocurrencies using the original scaled DataFrame.
- Create a copy of the original data and add a new column with the predicted clusters.
- Create a scatter plot using hvPlot as follows:
- Set the x-axis as "price_change_percentage_24h" and the y-axis as "price_change_percentage_7d".
- Color the graph points with the labels found using K-means.
- Add the "coin_id" column in the hover_cols parameter to identify the cryptocurrency represented by each data point.

**Results:**<font size=”1000”>

Visualize the Dataset

<img width="685" alt="image" src="https://user-images.githubusercontent.com/117549284/232964204-af438c21-713b-4f07-8b03-46dcec7d0ae2.png">

<img width="582" alt="image" src="https://user-images.githubusercontent.com/117549284/232964551-b3f83a79-44ed-4713-88ce-1984d3daea06.png">

Find the Best Value for k Using the Original Scaled DataFrame:

<img width="684" alt="image" src="https://user-images.githubusercontent.com/117549284/232964578-0d76adb5-4521-41d0-80d6-24f180b27c6b.png">
The best value for k is when k=2 where inertia declines the fastest

Cluster Cryptocurrencies with K-means Using the Original Scaled Data:

<img width="618" alt="image" src="https://user-images.githubusercontent.com/117549284/232964649-15b27ac6-09ca-44fa-aa90-e321364919c7.png">

3D Rendention of Cluster Cryptocurrencies with K-means Using the Original Scaled Data:

<img width="701" alt="image" src="https://user-images.githubusercontent.com/117549284/232964722-587ffe0e-b92a-4ec3-884a-ebd893f3c5b4.png">

Find the Best Value for k Using the PCA Data:

<img width="609" alt="image" src="https://user-images.githubusercontent.com/117549284/232964759-fd1a8663-ecaa-45dd-9013-1e880455c412.png">

The best value for k remains at when k=2 where inertia declines the fastest, same as the original data

Optimize Clusters with Principal Component Analysis:

<img width="609" alt="image" src="https://user-images.githubusercontent.com/117549284/232964829-d4071b25-7066-4fdf-9f5d-2bdc15a36765.png">

3D Rendention of Clusters with Principal Component Analysis:

<img width="710" alt="image" src="https://user-images.githubusercontent.com/117549284/232964896-996f9c05-6595-4392-94f1-f9cd4cffc5e5.png">

The effect of using fewer data in comparing Original Data vs PCA Data shows that PCA reduces the level of inertia (as shown when inertia declined form 8.2 x 10^6 to only 192). Using PCA, althought fewer data points, the optimization level remains the same which follows the principle of dimensionality reduction. PCA's data is more closely gathered together and easily visualized outliers. 
