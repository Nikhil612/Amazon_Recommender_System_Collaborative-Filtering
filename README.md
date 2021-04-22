## What is a recommendation system?

A recommendation engine is a system that suggests products, services, information to users based on analysis of data. 
Notwithstanding, the recommendation can derive from a variety of factors such as the history of the user and the behaviour of similar users.

## Our Idea To Do the Task in More Efficient Way -

We have build a robust recommender system for Amazon Products. 
We have used various Machine Learning algorithms and tested them. We have used Electronics dataset. 
This dataset has product id, which is a unique identifier for all products on amazon.com. It also contains the star rating given by each user identified by the user id.


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
<img src="https://user-images.githubusercontent.com/34812655/115681547-7cdfb180-a309-11eb-8eeb-583d7b41dd4a.png" width="100" height="100">
![image](https://user-images.githubusercontent.com/34812655/115681547-7cdfb180-a309-11eb-8eeb-583d7b41dd4a.png)



2. Collaborative filtering
   - Collaborative filtering using Singular value decomposition
     ![image](https://user-images.githubusercontent.com/34812655/115673650-b90f1400-a301-11eb-8397-65d1981edaef.png)

    - Collaborative filtering using KNN With means (user-user similarity)
      ![image](https://user-images.githubusercontent.com/34812655/115673343-5fa6e500-a301-11eb-9b29-194419f862c0.png)
      
     - Collaborative filtering using KNN With means (item-item similarity)
       ![image](https://user-images.githubusercontent.com/34812655/115673015-ff17a800-a300-11eb-9145-adfff5ccbb3c.png)
       

3. Hybrid Recommendor System

![image](https://user-images.githubusercontent.com/34812655/115671587-87954900-a2ff-11eb-820d-4fe95a2305a1.png)



