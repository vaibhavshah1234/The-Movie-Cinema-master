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

5.Open Heroku at your Dekstop , create a new app with app name (write app name you want) connect it with your Github profile find repositories and just deploy your model

6.Hurray! That's it.

# Architecture

![1](https://user-images.githubusercontent.com/69906280/119215237-042b6b00-baea-11eb-85e1-3aeef656bcbb.jpg)
