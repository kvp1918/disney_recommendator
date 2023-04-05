# Disney Content Recommendation System

This project built a recommendation system to recommend movies/shows based on a movie/show you like.

## Data
The data source was found on Kaggle [here](https://www.kaggle.com/datasets/victorsoeiro/disney-tv-shows-and-movies?select=credits.csv).

## Methods
For the recommendation system I used `genre`, `type`, `age certification`, and `runtime`.

The variables `genre`, `type`, `age certification` were one hot encoded and then the entire dataset was scaled. 

Since there was a mix of categorical and continuous data I used the Gower distance to calculate dissimilarity scores between each pair of movies/shows.

## Results
I converted the results into an interactive Shiny app with a reactable table. Select the movie/show you liked and you will get a list of 10 recomended movies/shows.

![](recomender_table.gif)
