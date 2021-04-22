## What is a recommendation system?

A recommendation engine is a system that suggests products, services, information to users based on analysis of data. 
Notwithstanding, the recommendation can derive from a variety of factors such as the history of the user and the behaviour of similar users.

## PROBLEM FACED BY CUSTOMERS -

Customers can spend hours scrolling through hundreds, sometimes thousands of items of merchandise never finding an item they like. Shoppers need to be provided suggestions based on their likes and needs in order to create a better shopping environment that boosts sales and increases the time spent on a website. This helps to boost their sales and also has better customer experience throughout the process.

## Idea To Do the Task in More Efficient Way -

To Build a Recommendor System that are beneficial to both service providers and users. They reduce transaction costs of finding and selecting items in an online shopping environment. Focus Area is Ecommerce, where recommender systems enhance revenues for the fact that they are effective means of selling more products. In scientific libraries, recommender systems support users by allowing them to move beyond catalog searches. Therefore, the need to use efficient and accurate recommendation techniques within a system that will provide relevant and dependable recommendations for users cannot be over-emphasized.


# DATASET USED TO ACHIEVE TASK
[ElctronicsProducts_Ratings_DATASET](http://jmcauley.ucsd.edu/data/amazon/)
**DOWNLOAD ELECTRONICS.tx.gz


PYTHON TO OBTAIN DATASET:
```
from os import path
if path.exists("ratings_Electronics.csv"):
    print ("Data Exists")
    Data=pd.read_csv('ratings_Electronics.csv',names=('userId','productId','ratings','timestamp'))
    print('Data Loaded')
else:
    os.system('curl http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/ratings_Electronics.csv -o ratings_Electronics.csv')
    print('Done downloading')
```


## Algorithms To Rescue

- [x] Popularity based
- [x] Collaborative filtering 
- [x] Hybrid Recommendation System

1. Popularity Based
<img src="https://user-images.githubusercontent.com/34812655/115681547-7cdfb180-a309-11eb-8eeb-583d7b41dd4a.png" width="200" height="200">



2. Collaborative filtering
   - Collaborative filtering using Singular value decomposition
   <img src="https://user-images.githubusercontent.com/34812655/115673650-b90f1400-a301-11eb-8397-65d1981edaef.png" width="200" height="200">
   

   - Collaborative filtering using KNN With means (user-user similarity)
   <img src="https://user-images.githubusercontent.com/34812655/115673343-5fa6e500-a301-11eb-9b29-194419f862c0.png" width="200" height="200">

      
   - Collaborative filtering using KNN With means (item-item similarity)
   <img src="https://user-images.githubusercontent.com/34812655/115673015-ff17a800-a300-11eb-9145-adfff5ccbb3c.png" width="200" height="200">
       

3. Hybrid Recommendor System

<img src="https://user-images.githubusercontent.com/34812655/115671587-87954900-a2ff-11eb-820d-4fe95a2305a1.png" width="200" height="200">

# RESULTS

## POPULARITY BASED
![image](https://user-images.githubusercontent.com/34812655/115682865-b9f87380-a30a-11eb-9cc8-000c6aa0cf58.png)


## COLLABORATIVE APPROACH

**ITEM-ITEM COLLABORATIVE**

![image](https://user-images.githubusercontent.com/34812655/115682938-ca105300-a30a-11eb-8c52-629c96d0b92a.png)

**USER-USER COLLABORATIVE**

![image](https://user-images.githubusercontent.com/34812655/115683078-ef9d5c80-a30a-11eb-8dcf-8d94da0336e5.png)

**Singular Value Decomposition**

![image](https://user-images.githubusercontent.com/34812655/115683272-21162800-a30b-11eb-80f8-42542d2569b6.png)


## HYBRID SYSTEM

![image](https://user-images.githubusercontent.com/34812655/115683629-7f430b00-a30b-11eb-81ba-29d0a1309437.png)




## References

[1]	https://towardsdatascience.com/web-scraping-recommender-systems-project-1d360fa678e4

[2]	https://towardsdatascience.com/how-to-build-a-model-based-recommendation-system-using-python-surprise-2df3b77ab3e5

[3]	https://towardsdatascience.com/deep-learning-based-recommender-systems-3d120201db7e

[4]	https://www.cs.umd.edu/~samir/498/Amazon-Recommendations.pdf

[5]	https://medium.com/@madasamy/introduction-to-recommendation-systems-and-how-to-design-recommendation-system-that-resembling-the-9ac167e30e95

[6]	https://towardsdatascience.com/product-recommender-using-amazon-review-dataset-e69d479d81dd






