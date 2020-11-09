<img src="https://github.com/nmshafie1993/RecommenderSystems/blob/master/Recommender%20system.jpeg" alt="RecommenderSystems"><br>
# Recommender Systems <br>
In this notebook, I practiced building different types of recommender systems using the Pandas library and various machine learning algorithms.<br>
<br>
## Part 1 - Popularity-Based Recommenders 
Our main goal in this section is to develop a recommender system that suggests restaurants to consumers. Initially, I started with 2 dataset from University of California, Irvine <a href="https://archive.ics.uci.edu/ml/datasets/Restaurant+%26+consumer+data"> "Restaurant & consumer data" </a>. To achieve my goal, I made a popularity-based recommender that works based on popularity of restaurants among users. The assumption is that the restaurant that has the highest counts of rating is the most popular. The downside to this method is that it cannot produce personalized results. By Looking at the rating counts, I found the top 5 popular places. Then, I looked out the cuisine of top 5 rated restaurant which turned out most of them are mexican. Looks <br>
 <br>
<img src="https://github.com/nmshafie1993/RecommenderSystems/blob/master/1.PNG" alt="table_1">
<br>
## Part 2 - Correlation-Based Recommenders
Here, I continue my efforts in building a recommender system that offers the best possible options to consumers. I decided to make a correlation-based recommender which Unlike popularity-based system, do take users preferences into account. In correlation-based recommendation systems, items are recommended based on users reviews. In other words, it chooses the items based on how well the items correlates with other items with respect to users ratings. Correlation-based recommendation systems use Pearson's R correlation to offer the items which are most similar to the past chosen items by users.<br>
In this section, I added another dataset from the <a href="https://archive.ics.uci.edu/ml/datasets/Restaurant+%26+consumer+data"> same source </a> which provides name, address, and other details about the restaurants. I seperated the place ID and name column to merge with the previous datasets. Then, I calculated the average rating that each place is given. I also counted the number of ratings for each place to see how popular each place is. I found that there has been 130 unique places that have been reviewed in the dataframe. A restaurant that called 'Tortas Locas Hipocampo' from mexican cuisine has the highest amount of ratings. I was curious to see what restaurants are the most similar to Tortas so I can recommend them to consumers. So, I canculated the correlation between user's rating to Tortas and other restaurants. I got a list of restaurants with their Pearson's R value. After careful post processing, I recommended Restaurante 'El Reyecito' to the users who like 'Tortas'. This process is reproducible with any other restaurant.<br>

## Part 3. Classification-Based Collaborative Filtering (Machine Learning Based Recommenders - Logistic Regression)
Here, I wanted to build a system that can help banks to decide which new users they should offer their banking system to. So, I developed a classification-based collaborative filtering system which is able to make personlized recommendations since it is taking into the account the users attributes as well as purchase history and other contextual data(e.g. browser history). The data of this section has been obtained from University of California, Irvine 

## Part 4. Collaborative Filtering System

## Part 5. Content_based Recommender


