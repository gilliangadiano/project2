# Top Youtube Channels #

Our project was to discover what a top YouTube channel looks like. In order to do this, we found a top 100 list of youtube channels on Kaggle that was organized by . Through that, we took their top 100 list and then scraped socialblade for their current data.

## App Description: ## 

We used the Kaggle YouTube datasets to identify the top 100 YouTube channels and then used the YouTube API to retrieve the information for these channels. The retrieved information was loaded to a SQLite database and a CSV file. The database is used by the Flask app to render the HTML pages and the CSV file is used by Tableau to generate the visualizations.


## Contents of the Git Repo: ##

### data: ###
    1) Top83_YouTube_Channels.csv: Channel information extracted using YouTube Data API.
    2) kaggle_data.csv: Used this dataset to shortlist the top 100 youtube channels based on their rank.


### db:
1) YouTube_Top_Channels.sqlite: database containing the top 83 youtube channels retrieved with the YouTube API.

static: 
-------
contains the css and js components:

    a) css folder:
        1) bootstrap.min.css: Our website's bootstrap css
        2) style.css: our website's css

    b) js folder: 
        1) logic.js: javascript to add interactivity to pages.


templates: 
----------
contains the HTML pages:
    1) challenges.html
    2) data.html
    3) index.html: landing page
    4) money.html
    5) visualization_1.html
    6) visualization_2.html
    7) visualization_3.html


Flask app:
-----------
app.py: This is the app that hands off the data from our CSV and JSON to the website. 


Tableau visualizations:
------------------------
youtube_book.twb: This is our Tableau notebook. 

Jupyter Notebooks:
---------------------
    1) YouTube_Data_Integration.ipynb





# project2