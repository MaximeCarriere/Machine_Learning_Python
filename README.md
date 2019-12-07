# Machine_Learning_Python
## 1) KMean 
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


Kmean is a technic used in classification or regression. It is based on the metric distance of the new data with the matrix of existing data. 
- Distance metric (typically Euclidian) 
- How many nearest neighbors (1-2-3.... here we will use 5) 
- Optional weighting function (Ignored) 
- Method for agrregating classes of neighbor (Majority vote) 

The K-mean methods creates clusters based on the data. In our dataset we have matrix of 30 dimensions, all are included into the analysis. The demonstration of K-means is as follows : 

![Screen Shot 2019-12-07 at 13 18 20](https://user-images.githubusercontent.com/55028120/70374556-1fa1b680-18f4-11ea-89db-4fa2bbf6c20b.png)


(From Wikipedia page : https://en.wikipedia.org/wiki/K-means_clustering) 

