# The-VS-Movie-Cinema

Content Based Recommender System recommends movies similar to the movie user likes and analyses the sentiments on the reviews given by the user for that movie.

The details of the movies(title, genre, runtime, rating, poster, etc) are fetched using an API by TMDB, https://www.themoviedb.org/documentation/api, and using the IMDB id of the movie in the API, I did web scraping to get the reviews given by the user in the IMDB site using beautifulsoup4 and performed sentiment analysis on those reviews.

Link to "The VS Movie Cinema" application:https://the-vs-movie-cinema.herokuapp.com/

# How to get the API key?
Create an account in https://www.themoviedb.org/, click on the API link from the left hand sidebar in your account settings and fill all the details to apply for API key. If you are asked for the website URL, just give "NA" if you don't have one. You will see the API key in your API sidebar once your request is approved.

# How to run the project?
1.Clone or download this repository to your local machine.

2.Install all the libraries mentioned in the requirements.txt file with the command pip install -r requirements.txt

3.Get your API key from https://www.themoviedb.org/. (Refer the above section on how to get the API key)

4.Replace YOUR_API_KEY in both the places (line no. 23 and 43) of static/recommend.js file and hit save.

5.Open Heroku on your Dekstop , create a new app with app name (write app name you want) connect it with your Github profile, find repositories and just deploy your model

6.Hurray! That's it.

# Architecture

![1](https://user-images.githubusercontent.com/69906280/119215237-042b6b00-baea-11eb-85e1-3aeef656bcbb.jpg)

Similarity Score :
How does it decide which item is most similar to the item user likes? Here we use the similarity scores.

It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.

How Cosine Similarity works?
Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.


![2](https://user-images.githubusercontent.com/69906280/119225502-be8a9480-bb21-11eb-8170-339676a042cd.png)


More about Cosine Similarity  :https://www.machinelearningplus.com/nlp/cosine-similarity/

                                
