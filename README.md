# **Model Based Collaborative Filtering**

This method's core concept is dimensional reduction. Matrix factorization will be used to do model-based collaborative filtering. Singular Value Decomposition (SVD), Alternating Least Square (ALS), and Weighted Alternating Least Square (WALS) are three matrix factorization alternatives that can be utilized in collaborative filtering (WALS). <br>

![image](https://user-images.githubusercontent.com/73176284/167830660-f1a996e5-4166-42d5-9e33-9a1b03c0774c.png)

Matrix factorization is a technique for dividing a huge matrix into two smaller ones. We start with a 5 x 4 matrix in the following example. This matrix is divided into two smaller matrices. 5 x 2 is the first matrix. The matrix describes the user's hidden features. The items matrix, which measures 2 x 4, is the second matrix. This matrix describes the film's hidden qualities. In the following approach, we anticipate how much a user will rate a specific item. The value of user 4's first latent factor (10) is multiplied by the value of the interstellar film's first latent factor (1), plus the value of user 4's second latent factor (1) multiplied by the value of the interstellar film's second latent component (1). (-3). The result of the rating forecast is a 7. This is how you may estimate a product's user rating.

# **Surprise**
<p align="center">
  <img width="450" height="300" src="https://raw.githubusercontent.com/NicolasHug/Surprise/master/logo_black.svg">
</p>
Surprise is a Python scikit for building and analyzing recommender systems that deal with explicit rating data. Surprise was designed with the following purposes in mind:<br>

- Give users perfect control over their experiments. To this end, a strong emphasis is laid on documentation, which we have tried to make as clear and precise as possible by pointing out every detail of the algorithms.
- Alleviate the pain of Dataset handling. Users can use both built-in datasets (Movielens, Jester), and their own custom datasets.
- Provide various ready-to-use prediction algorithms such as baseline algorithms, neighborhood methods, matrix factorization-based ( SVD, PMF, SVD++, NMF), and many others. Also, various similarity measures (cosine, MSD, pearson...) are built-in.
- Make it easy to implement new algorithm ideas.
- Provide tools to evaluate, analyse and compare the algorithms' performance. Cross-validation procedures can be run very easily using powerful CV iterators (inspired by scikit-learn excellent tools), as well as exhaustive search over a set of parameters.

The name Surprise stands for Simple Python RecommendatIon System Engine. Please note that surprise does not support implicit ratings or content-based information. For more information, please click this link: [**Surprise Documentation**](http://surpriselib.com/)

# **E-commerce Product Recommendation with Surprise**
<p align="center">
  <img width="470" height="300" src="https://user-images.githubusercontent.com/73176284/167834481-bec3e153-f0ee-4216-a21f-5edbb67f0f68.jpg">
</p>

To experiment with recommendation algorithms, we will need data that contains a set of items and a set of users who have reacted to some of the items. The reaction can be explicit (rating on a scale of 1 to 5, likes or dislikes) or implicit (viewing an item, adding it to a wish list, the time spent on an article). While working with such data, you’ll mostly see it in the form of a matrix consisting of the reactions given by a set of users to some items from a set of items. Each row would contain the ratings given by a user, and each column would contain the ratings received by an item.<br>

The goal of this project is to develop a recommendation system that will be customized for each user, ensuring that every item purchased is suitable with their tastes.

## **Conclusion**
![image](https://user-images.githubusercontent.com/73176284/167832858-d77ff252-e479-42e0-9add-75233c9cd2e8.png)
- Plasters In Tin Circus Parade, 6 Rocket Balloons, Red Toadstool Led Night Light, and Rabbit Night Light are the products to recommend for Customer 12509 (Emmet Piggens).
- Red Toadstool Led Night Light, Rabbit Night Light, Plasters In Tin Circus Parade, and 6 Rocket Balloons are the products to recommend for Customer 12681 (Claudetta Guirau).
- Plasters In Tin Circus Parade, Red Toadstool Led Night Light, Rabbit Night Light, and 6 Rocket Balloons are the products to recommend for Customer 12683 (Jaquelyn Eckh).
