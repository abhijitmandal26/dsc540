### Covid 19 Data Analysis and Comparison
![image](https://user-images.githubusercontent.com/13950516/162676269-ab24f4ed-7089-44de-bc64-64c2ae6b0710.png)


### Context
The novel coronavirus, also known as SARS-CoV-2, is a contagious respiratory virus that first reported in Wuhan, China. On 2/11/2020, the World Health Organization designated the name COVID-19 for the disease caused by the novel coronavirus. This new strain of virus has strike fear in many countries as cities are quarantined and hospitals are overcrowded. 
This project aims at exploring COVID-19 through data analysis and visualization.

### <img src="https://user-images.githubusercontent.com/13950516/162672483-4d953e53-2d6b-49d6-81ba-e7daa4a54351.png" width="40" height="40" /> &nbsp; Problem Statement:

#### Some of the questions that we are looking to solve here are:

- How do we define a tumor as malignant or benign ?
- Can any benign tumor turn to malignant at later time ?
- What are the characteristics of a malignant and benign tumor (size, mass, texture, smoothness etc)?
- Does the chances of a breast cancer varies from individual to individual?

![image](https://user-images.githubusercontent.com/13950516/162662239-6c732024-3b3e-4b3e-90e9-ba7c32b791cb.png)


### <img src="https://user-images.githubusercontent.com/13950516/162672846-869bf047-63a7-489f-9b33-4f4a3beab1b2.png" width="40" height="40" /> &nbsp; Dataset
The dataset is taken from https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29

### <img src="https://user-images.githubusercontent.com/13950516/162673233-e0f5d3ac-ccf7-430e-9a56-46e202098648.png" width="40" height="40" />&nbsp; Variable Descriptions

diagnosis --> The diagnosis of breast tissues (M = malignant, B = benign)

radius_mean --> mean of distances from center to points on the perimeter

texture_mean --> standard deviation of gray-scale values

perimeter_mean --> mean size of the core tumor

smoothness_mean --> mean of local variation in radius lengths

compactness_mean --> mean of perimeter^2 / area - 1.0

concavity_mean --> mean of severity of concave portions of the contour

concave points_mean --> mean for number of concave portions of the contour

fractaldimensionmean --> mean for "coastline approximation" - 1

radius_se --> standard error for the mean of distances from center to points on the perimeter

texture_se --> standard error for standard deviation of gray-scale values

smoothness_se --> standard error for local variation in radius lengths

compactness_se --> standard error for perimeter^2 / area - 1.0

concavity_se --> standard error for severity of concave portions of the contour

concave points_se --> standard error for number of concave portions of the contour

fractaldimensionse --> standard error for "coastline approximation" - 1

radius_worst --> "worst" or largest mean value for mean of distances from
center to points on the perimeter

texture_worst --> "worst" or largest mean value for standard deviation of gray-scale values

smoothness_worst --> "worst" or largest mean value for local variation in radius lengths

compactness_worst --> "worst" or largest mean value for perimeter^2 / area - 1.0

concavity_worst --> "worst" or largest mean value for severity of concave portions of the contour

concave points_worst --> "worst" or largest mean value for number of concave portions of the contour

fractaldimensionworst--> "worst" or largest mean value for "coastline approximation" - 1

### <img src="https://user-images.githubusercontent.com/13950516/162673345-5ea37d71-b9e4-47b7-aa6e-c43921d7b2d0.png" width="40" height="40" />&nbsp; Approach

We will first analyze the data and look for any cleanups needed, then we will derive correlation between the variables, after visualizing and analyzing the data we will use machine learning algorithm KNN to derive at a conclusion.

I have considered variables such as tumor size, mass, texture, smoothness, thickness etc that can help in predicting the chances of a tumor being malignant or benign, 

I have used K-nearest neighbor algorithm to classify the tumor, the result of this algorithm provided an accurate response.

<img width="420" alt="image" src="https://user-images.githubusercontent.com/13950516/162662282-ad502e34-3b56-4690-9b04-234091bd4ab7.png">

### <img src="https://user-images.githubusercontent.com/13950516/162673481-c1ce4edf-5240-43be-ae07-e7ef061be0c6.png" width="40" height="40" />&nbsp; Conclusion

We have features of a tumor but I was not sure what does they mean or actually how much do we need to know about these features I believe that we do not need to know meaning of these features however in order to imagine in our mind we should know something like variance, standard deviation, number of sample (count) or max min values. 

These type of information helps to understand about what is going on data. For example , the question is appeared in my mind the area_mean feature’s max value is 2500 and smoothness_mean features’ max 0.16340. Also, it would have been great if i could compare the result of my data model vs other machine learning algorithms like Random Forest, SVM etc. 

In future we can look into the implementation of artificial neural net and deep learning for predictive model development with a larger and un- structured data set. 
This will use unsupervised learning algorithms such SVM etc. to first label the data and distributing them over training set, cross-validation set and test set.
