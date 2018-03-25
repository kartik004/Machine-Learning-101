# Introduction to K-nearest neighbor classifier
K-nearest neighbor classifier is one of the introductory supervised classifier, which every data science learner should be aware of. Fix & Hodges proposed K-nearest neighbor classifier algorithm in the year of 1951 for performing pattern classification task.

For simplicity, this classifier is called as Knn Classifier. To be surprised k-nearest neighbor classifier mostly represented as Knn, even in many research papers too. Knn address the pattern recognition problems and also the best choices for addressing some of the classification related tasks.

The simple version of the K-nearest neighbor classifier algorithms is to predict the target label by finding the nearest neighbor class. The closest class will be identified using the distance measures like Euclidean distance.

## Knn classification application
Let’s assume a money lending company “XYZ” like UpStart, IndiaLends, etc. Money lending XYZ company is interested in making the money lending system comfortable & safe for lenders as well as for borrowers. The company holds a database of customer’s details.

Using customer’s detailed information from the database, it will calculate a credit score(discrete value) for each customer. The calculated credit score helps the company and lenders to understand the credibility of a customer clearly. So they can simply take a decision whether they should lend money to a particular customer or not.

###The customer’s details could be:

* Educational background details.
    * Highest graduated degree.
    * Cumulative grade points average (CGPA) or marks percentage.
    * The reputation of the college.
    * Consistency in his lower degrees.
    * Whether to take the education loan or not.
    * Cleared education loan dues.
* Employment details.
  * Salary.
  * Year of experience.
  * Got any onsite opportunities.
  * Average job change duration.

The company(XYZ) use’s these kinds of details to calculate credit score of a customer. The process of calculating the credit score from the customer’s details is expensive. To reduce the cost of predicting credit score, they realized that the customers with similar background details are getting a similar credit score.

So, they decided to use already available data of customers and predict the credit score using it by comparing it with similar data. These kinds of problems are handled by the k-nearest neighbor classifier for finding the similar kind of customers.

## Knn Algorithm Pseudocode:
  1. Calculate “d(x, xi)” i =1, 2, ….., n; where d denotes the Euclidean distance between the points.
  2. Arrange the calculated n Euclidean distances in non-decreasing order.
  3. Let k be a +ve integer, take the first k distances from this sorted list.
  4. Find those k-points corresponding to these k-distances.
  5. Let ki denotes the number of points belonging to the ith class among k points i.e. k ≥ 0
  6. If ki >kj ∀ i ≠ j then put x in class i.
  
[KNN Implementation](https://github.com/kartik004/Machine-Learning-101/blob/master/KNN/KNN%20Implementation%20using%20python.ipynb)
