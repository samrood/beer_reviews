## Binary Classification on Beer Reivews
My overall objective of this porject is to use user reviews on beers from BeerAdvocate to predict if a user will enjoy a beer type or not based on their other reviews. 


### Data Collecting and Cleaning - noteboook 
The first notebook will 
- collect beer reviews data from kaggle
- do an inital clean of the data 
- save the newwly cleaned data in a database in SQL on my AWS to access in future notebooks
- group beer types: 
    - Since there are so many beer types that are very similar to each other, here we are going to group types together to simplify the classification. Doing some reseach this is the grouping I have come up with:



### Features to be made: 
User features to make:
   - total number of reviews the user has done: user_total_review_count  
   
 _user-type features_ -
   - number of reviews for each type by user: user_type_review_count
   - ratio of reviews of type compared to total reviews: user_review_type_ratio 
   - number of types of beers user has reviewed: user_review_number_of_types  
   - average overall rating for each beer type: user_avg_overall_rating_of_type
   - average apperance rating for each beer type: user_avg_apperance_rating_of_type
   - average aroma rating for each beer type: user_avg_aroma_rating_of_type
   
  _user-beer features_ -
   - number of reviews for each type by user: user_beer_review_count
   - ratio of reviews of type compared to total reviews: user_review_beer_ratio 
   - number of types of beers user has reviewed: user_review_number_of_beers  
   - average overall rating for each beer type: user_avg_overall_rating_of_beer 
   
   _user-brewery features_ - 
   - number of breweries user has reviewed: user_review_number_of_breweries
   - number of reviews for each brewery by user: user_brewery_review_count
   - ratio of reviews of brewery compared to total: user_review_brewery_ratio
   - average overall rating for each brewery: user_avg_overall_rating
        
Beer features to make:
   - total number of reviews for each beer: beer_total_review_count
   - average overall rating for each beer: beer_avg_rating
    
Beer type features to make:
   - total number of reviews for each beer type: type_total_review_count
   - average overall rating for each type: type_avg_rating 

Brewery features to make:
   - total number of reviews for each brewery: brewery_total_review_count
   - average overall rating for each brewery: brewery_avg_overall_rating 



### Creating model - notebook 
The purpose of this notebook is to:
- obtain the data from AWS
- create features
- create model to predict if use will/wont enjoy a beer type
- train/test and evaluate the models
- plot models
- create new features to improve model
