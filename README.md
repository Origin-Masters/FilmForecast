# FilmForecast
Project aiming at Predicting Movie Ratings using Methods of Machine Learning

# Topic : Predict the Rating of Movies

### The goal in this project is to predict the rating (vote_average) of movies based on other features (e.g., their release date and box-office revenue).

#### Data :

The TMDB Movies Dataset consists of information about 1 million movies scraped from IMDB. The dataset is available for download from Moodle. More information about the dataset can be found here:

https://www.kaggle.com/datasets/asaniczka/tmdb-movies-dataset-2023-930k-movies/data

#### Goals :

Employing the methods that we covered in the lecture, you should come up with your own solution to the problem and evaluate it. In order to obtain bonus points, you have to submit your solution as a single Jupyter Notebook by August 30, 2025. Your Jupyter notebook should cover the following aspects:

some analysis of the dataset (e.g., statistics regarding its size or the distribution of individual features)
details on any preprocessing that you applied to the dataset (e.g., to clean it up by removing null values)
a detailed description of your approach (e.g., which method to do you use, which features do you consider)
a discussion of the experimental results (e.g., what is the performance that your achieves, how does it compare to other methods)


## Our Approach :

At first, Using a Linear Regression and `excluding` the unrated movies (Rating == 0) we obtained :

```
📊 Validation R2: 0.05239199004077433
----------------------
📊 Test R2: 0.05341469876521021
----------------------
📉 Validation MSE: 3.756533272317015
----------------------
📉 Test MSE: 3.7099452036246263
----------------------

With few examples -> only train on a subset of the data, less statistical power
When target variance shrinks, R² naturally drops if the model can’t explain much variation 
```

Trying out Lasso Regression, we obtained the results:
```
- Train MSE: 4.6666
- Validation MSE: 4.6926
- Test MSE: 4.6840
```



