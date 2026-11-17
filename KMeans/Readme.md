# Introduction to K-Means Clustering

**K-Means Clustering** is an unsupervised machine learning algorithm used to group similar data points into clusters.

It divides the dataset into a fixed number of groups (K), where each group contains data points that are similar to each other.

**Example:** Grouping customers based on their shopping habits, income, and spending patterns.

##  What is K-Means Clustering?

K-Means is a clustering algorithm that groups data points based on their similarity.

It works by:
- Selecting the number of clusters (K).
- Finding the center point of each cluster.
- Assigning each data point to its nearest cluster center.
- Updating the cluster centers until they stop changing significantly.

![K-Means Clustering](https://th.bing.com/th/id/OIP.eNWN14P6oQwySgxLuMqB9gHaDv?r=0&o=7rm=3&rs=1&pid=ImgDetMain&o=7&rm=3)

## Important Terms in K-Means

### 1. K (Number of Clusters)

K represents the number of groups we want to create.

Example: If K = 3, the algorithm divides the dataset into three clusters.

### 2. Centroid

A centroid is the center point of a cluster.

It is calculated by taking the average of all data points belonging to that cluster.

### 3. Cluster

A cluster is a group of data points that are similar to each other.

## How Does K-Means Work?

K-Means works by repeatedly assigning data points to the nearest centroid and updating the centroids.

### Steps Involved:

1. **Choose K:** Decide how many clusters are required.
2. **Initialize Centroids:** Select K initial centroids from the dataset.
3. **Assign Data Points:** Assign each data point to its nearest centroid.
4. **Update Centroids:** Calculate the mean of the data points in each cluster to find new centroids.
5. **Repeat:** Repeat the assignment and update steps until the centroids stop changing significantly.
6. **Final Clusters:** The algorithm produces the final groups of similar data points.

##  K-Means Formula

The centroid of a cluster is calculated using the mean of its data points.

$\displaystyle C = \frac{x_1 + x_2 + \cdots + x_n}{n}$

**Where:**

- `C` = New centroid.
- `x` = Data points in the cluster.
- `n` = Total number of data points.

### Euclidean Distance

K-Means commonly uses Euclidean distance to find the nearest centroid.

$\displaystyle d = \sqrt{(x_2-x_1)^2 + (y_2-y_1)^2}$

**Where:**

- `d` = Distance between two points.
- `x₁, y₁` = Coordinates of the first point.
- `x₂, y₂` = Coordinates of the second point.

## 6. How to Choose the Best K Value?

The **Elbow Method** helps find a suitable number of clusters.

### Steps:

1. Run K-Means with different K values.
2. Calculate the Within-Cluster Sum of Squares (WCSS) for each K.
3. Plot K values against WCSS.
4. Find the point where the decrease in WCSS starts slowing down. This point looks like an elbow.
5. Choose that K value as a suitable number of clusters.

##  Important Parameters of KMeans()

### 1. n_clusters

- Specifies the number of clusters to create.
- Example: `n_clusters=3` creates three clusters.

### 2. init

- Specifies the method used to select initial centroids.
- Common options:
  - `k-means++`
  - `random`

### 3. n_init

- Specifies how many times the algorithm runs with different initial centroids.
- The best result is selected based on inertia.

### 4. max_iter

- Specifies the maximum number of iterations for each run.

### 5. random_state

- Controls randomness to help produce reproducible results.

##  Advantages of K-Means

- Simple and easy to understand.
- Easy to implement.
- Works well with large datasets.
- Fast compared to many clustering algorithms.
- Helps discover hidden patterns in data.

##  Disadvantages of K-Means

- Requires the number of clusters (K) in advance.
- Sensitive to initial centroid selection.
- Sensitive to outliers.
- Does not work well with irregularly shaped clusters.
- Feature scaling is important when features have different ranges.
