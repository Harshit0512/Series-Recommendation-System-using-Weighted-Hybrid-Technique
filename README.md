# Series Recommendation System Using Weighted Hybrid Technique

![Python](https://img.shields.io/badge/Python-3.8.2-blueviolet)
![Numpy](https://img.shields.io/badge/Numpy-1.16.4-red)
![Pandas](https://img.shields.io/badge/Pandas-0.24.2-green)
![Seaborn](https://img.shields.io/badge/Seaborn-0.9.0-fcba03)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.1.0-blue)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-darkorange)
![Sklearn](https://img.shields.io/badge/Sklearn-0.21.2-darkviolet)

Recommender system becomes very popular and has important role in an information system or webpages nowadays. A recommender system tries to make a prediction of which item a user may like based on his activity on the system.

The recommendation system in this notebook is based on the IMDb rating system. IMDb had a special equation that weighs the votes.

**Formula Used-**<br>
<br>
<img  alt="PNG" width="500px" src="https://github.com/Harshit0512/Series-Recommendation-System-using-Weighted-Hybrid-Technique/blob/main/Images/formula%20of%20weighted%20average.png" /><br>
* This is a type of **collaborative filtering recommender systems**.
## DataSet
Dataset Used from Kaggle - [Web Series: Ultimate Collection](https://www.kaggle.com/amritvirsinghx/web-series-ultimate-edition)

Download Data - [Download Dataset](https://www.kaggle.com/amritvirsinghx/web-series-ultimate-edition/download)

## Resources Used
* **Jupyter**
* **Python-3.8.2**
* **Numpy-1.16.4**
* **Pandas-0.24.2**
* **Matplotlib-3.1.0**
* **Seaborn-0.9.0**
* **Sklearn-0.21.2**

## Data
* **Series Title** - Name of the TV Series
* **Year Released** - Released Year of TV Series
* **Content Rating** - PG Rating of Content
* **IMDB Rating** - Rating from IMDB Site
* **R Rating** - Rotton Tomato Rating
* **Genre** - Genre of the TV Show
* **Description** - Synopsis of the title
* **No of Seasons** - Total no of seasons
* **Streaming Platform** - Streaming service currently streaming on

## Data Cleaning and EDA
* Added **Series ID** into the dataset.
* Replacing all **nan** values with **unknown**.
* Extracting the number from string in column **No of Seasons**.
* Giving the proper name to the columns.
* Making **Series Title** into lowercase and use strip() to remove extra spaces.

* After applying formula we add column called **score** in the dataset.(score column has value which we computed for different series)

* Created new DataFrame having features listed below.

## Feature Selected 
* Series_Title
* score
* Content_Rating
* IMDB_Rating
* Genre
* No_of_Seasons
* Streaming_Platform

## Data Visualization
* **Popular Series with respect to IMDB Rating**<br>
<img  alt="PNG" width="700px" src="https://github.com/Harshit0512/Series-Recommendation-System-using-Weighted-Hybrid-Technique/blob/main/Images/popular_by_imdb_rating.png" /><br>

* **Popular Series with respect to Rotten Tomatoes Rating**<br>
<img  alt="PNG" width="700px" src="https://github.com/Harshit0512/Series-Recommendation-System-using-Weighted-Hybrid-Technique/blob/main/Images/popular_by_rotten_tomatoes.png" /><br>

* **Best Series with respect to the weighted Average**<br>
<img  alt="PNG" width="700px" src="https://github.com/Harshit0512/Series-Recommendation-System-using-Weighted-Hybrid-Technique/blob/main/Images/best_series.png" /><br>

* **Best Series with respect to the calculated score**<br>
<img  alt="PNG" width="700px" src="https://github.com/Harshit0512/Series-Recommendation-System-using-Weighted-Hybrid-Technique/blob/main/Images/best_shows_by_scores.png" /><br>

## Output
**Example** - If you go with **Stranger Things**
The recommended series for you:-<br>

<img  alt="PNG" width="700px" src="https://github.com/Harshit0512/Series-Recommendation-System-using-Weighted-Hybrid-Technique/blob/main/Images/example.png" /><br>

* If you searching for a series and it is not present in dataset then you will get message:- <br>

<img  alt="PNG" width="700px" src="https://github.com/Harshit0512/Series-Recommendation-System-using-Weighted-Hybrid-Technique/blob/main/Images/series_not_there.png" /><br>
