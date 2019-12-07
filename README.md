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

In pattern recognition, the k-nearest neighbors algorithm (k-NN) is a non-parametric and supervised method used for classification and regression. In both cases, the input consists of the k closest training examples in the feature space. The output depends on whether k-NN is used for classification or regression:

   -In k-NN classification, the output is a class membership. An object is classified by a plurality vote of its neighbors, with the object being assigned to the class most common among its k nearest neighbors (k is a positive integer, typically small). If k = 1, then the object is simply assigned to the class of that single nearest neighbor.
   -In k-NN regression, the output is the property value for the object. This value is the average of the values of k nearest neighbors.
K-nearest neighbors is a technic used in classification or regression. It is based on the metric distance of the new data with the matrix of existing data. 

Here we will compare the results with k=1 and k=5

The K-nearest neighbors methods creates clusters based on the data. In our dataset we have matrix of 30 dimensions, all are included into the analysis. The demonstration of K-nearest neighbors is as follows : 

![Screen Shot 2019-12-07 at 13 18 20](https://user-images.githubusercontent.com/55028120/70374556-1fa1b680-18f4-11ea-89db-4fa2bbf6c20b.png)


(From Wikipedia page : https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm 

### Results 

![k_meanaa](https://user-images.githubusercontent.com/55028120/70374666-59bf8800-18f5-11ea-8d45-8a1ef044dab0.png)


We observe that with k=1, the prediciton match perfectly the training data set and predicts quite well the test data set. With k=5, the model is less robust for the training data set but seems better for the test data set. There is no rules for the value of K but:
- A small value of k means that noise will have a higher influence on the result.
- A large value make it computationally expensive. 
Data scientists usually choose as an odd number (avoid confusion between two classes) if the number of classes is 2 and another simple approach to select k is set k=sqrt(n).


To go further ==> https://projecteuclid.org/download/pdfview_1/euclid.aos/1223908087

