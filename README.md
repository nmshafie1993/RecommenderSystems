<img src="https://github.com/nmshafie1993/RecommenderSystems/blob/master/Recommender%20system.jpeg" alt="RecommenderSystems"><br>
# Recommender Systems <br>
In this notebook, I practiced building different types of recommender systems <br>
## Part 1 - Popularity-Based Recommenders 
Initially, I started with 2 dataset from University of California, Irvine <a href="https://archive.ics.uci.edu/ml/datasets/Restaurant+%26+consumer+data"> "Restaurant & consumer data" </a>. <br>
### datasets information: 
1. <strong> rating_final.csv </strong> <br>
<ul> Instances: 1161 </ul>
<ul> Attributes: 5 </ul>
<ul> userID: Nominal </ul>
<ul> placeID: Nominal </ul>
<ul> rating: Numeric, 3 [0,1,2] </ul>
<ul> food_rating: Numeric, 3 [0,1,2] </ul>
<ul> service_rating: Numeric, 3 [0,1,2] </ul>

2. <strong> chefmozcuisine.csv </strong>
<ul> Instances: 916 </ul>
<ul>Attributes: 2 </ul>
<ul> placeID: Nominal </ul>
<ul> Rcuisine: Nominal, 59 [Afghan,African,American,Armenian,Asian,Bagels,Bakery,Bar,Bar_Pub_Brewery,Barbecue,Brazilian,Breakfast-Brunch,Burgers,Cafe-Coffee_Shop, Cafeteria,California,Caribbean,Chinese,Contemporary,Continental-European,Deli-Sandwiches,Dessert-Ice_Cream,Diner,Dutch-Belgian,Eastern_European,Ethiopian,Family,Fast_Food,Fine_Dining,French,,Game,German,Greek,Hot_Dogs, International,Italian,Japanese,Juice,Korean,Latin_American,Mediterranean,Mexican,Mongolian,Organic-Healthy,Persian, Pizzeria,Polish,Regional,Seafood,Soup,Southern,Southwestern,Spanish,Steaks,Sushi,Thai,Turkish,Vegetarian,Vietnamese] </ul>

### What I did:
I made a popularity-based recommender that works based on popularity of restaurants among users. The assumption is that the restaurant that has the highest counts of rating is the most popular. This method cannot produce personalized results. By Looking at the rating counts, I found the top 5 popular placed. Then, I looked out the cuisine of top 5 rated restaurant which turned out most of them are mexican. 
<img src="https://github.com/nmshafie1993/RecommenderSystems/blob/master/1.PNG" alt="table_1">

## Part 2 - Correlation-Based Recommenders
<br>
a popularity-based recommender using Pandas library that can recommend similar items based on correlation. </br>
<br> Also, we deploy various machine learning algorithms such nearest neighbors and logistic regression to make recommendations and evaluate our recommender system. </br>
