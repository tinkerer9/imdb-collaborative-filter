# IMDB Collaborative Filter

This program uses cosine similarity to predict which movies you will like based on what movies other users on IMDB like.

View the notebook here on [GitHub](https://github.com/tinkerer9/imdbcollaborativefilter/blob/main/IMDB_Collaborative_Filter.ipynb) or run it on [Google Colab](https://colab.research.google.com/github/tinkerer9/imdb-collaborative-filter/blob/main/IMDB_Collaborative_Filter.ipynb).

## Intended use

The user may like some movies but not others and will rate them on a scale from 1 to 5 (fractions allowed).
If they haven't seen the movie, they will leave the field blank.
The program will:

1.   Find similar users based off of (seen) movies
2.   Use those similar users to predict how the user would rate the unseen movies

This is known as **collaborative filtering**.

## Collaborative filtering

[Collaborative filtering](https://en.wikipedia.org/wiki/Collaborative_filtering) is a method of making predictions (filtering) about the interests of a user by collecting information from many other users (collaborative).

## Data source

The data in this project come from two CSV files from [IMDB](https://imdb.com): [`movies.csv`](https://github.com/tinkerer9/imdbdataset/blob/main/movies.csv) and [`ratings.csv`](https://github.com/tinkerer9/imdbdataset/blob/main/ratings.csv).
If the files are not found, the program automatically downloads them.
See more at [`getIMDBRatings()`](https://colab.research.google.com/drive/1H-imyPHMtxoq_W3JoGZcy9bvqyZn_9GD#scrollTo=Tasu3gTy8Wqe).
