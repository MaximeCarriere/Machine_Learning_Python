# Machine_Learning_Python
## 1) K-nearest neighbors
### Data and Goal


The data are from the Breast Cancer Wisconsin (Diagnostic) Database.

The goal is to create a classifier that can help diagnose patients.

    Data Set Characteristics:

    -Number of Instances: 569
    -Number of Attributes: 30 numeric, predictive attributes and the class
    -Attribute Information:
        - radius (mean of distances from center to points on the perimeter)
        - texture (standard deviation of gray-scale values)
        - perimeter
        - area
        - smoothness (local variation in radius lengths)
        - compactness (perimeter^2 / area - 1.0)
        - concavity (severity of concave portions of the contour)
        - concave points (number of concave portions of the contour)
        - symmetry 
        - fractal dimension ("coastline approximation" - 1)
        - class:
                - WDBC-Malignant (0)
                - WDBC-Benign (1)

 
### K-nearest neighbors explanation 

K-nearest neighbors is a technic used in classification or regression. It is based on the metric distance of the new data with the matrix of existing data. 
- Distance metric (typically Euclidian) 
- How many nearest neighbors (1-2-3.... here we will compare the results with k=1 and k=5) 
- Optional weighting function (Ignored) 
- Method for agrregating classes of neighbor (Majority vote) 

The K-nearest neighbors methods creates clusters based on the data. In our dataset we have matrix of 30 dimensions, all are included into the analysis. The demonstration of K-means is as follows : 

![Screen Shot 2019-12-07 at 13 18 20](https://user-images.githubusercontent.com/55028120/70374556-1fa1b680-18f4-11ea-89db-4fa2bbf6c20b.png)


(From Wikipedia page : https://en.wikipedia.org/wiki/K-means_clustering) 

### Results 

![k_meanaa](https://user-images.githubusercontent.com/55028120/70374666-59bf8800-18f5-11ea-8d45-8a1ef044dab0.png)


We observe that with k=1, the prediciton match perfectly the training data set and predicts quite well the test data set. With k=5, the model is less robust for the training data set but seems better for the test data set. 

