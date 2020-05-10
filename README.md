# What the animates and the inanimates are saying about Airbnb in San Francisco and Austin
<p align="center">
  <img src="https://i2.wp.com/www.contemporist.com/wp-content/uploads/2020/03/modern-circle-headboard-bedroom-design-backlit-180320-1112-01.jpg">
</p>
This repository contains code analyzing San-Francisco and Austin data from 2020. 

Data can be found [here](http://insideairbnb.com/get-the-data.html).

A blog post summarizing more details can be found [here](https://medium.com@imizezekwhat-the-animates-and-the-inanimates-are-saying-about-airbnb-in-san-francisco-and-austin-9705f7abf7bf

### Table of Contents
1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Data](#data)
4. [Running the code](#running)
5. [Results](#results)
6. [Acknowledgements](#acknowledgements)

### Introduction<a name="introduction"></a>
In this repository, I shall be analyzing AirBnB calendar data of Austin and San-Francisco from January, 2020 to December, 2020. Also the listing and review data. The aim of this project is to gain useful insight from the data and solve certain problems via questions:

1. Which cities have more expensive homestay across different times of the year(Austin or San Francisco) per availability?
2. Do I stand the chance to incur more costs on the request for additional services?
3. Joshua plans for vacation, where will he obtain better services for a price of 200 dollars per day: SF or Austin?
4. In the situation whereby Joshua's plan changes, which of the cities is more lenient with the cancellation policy?
5. Which of the room types is popular in San Francisco versus Austin?
5. What are property renters saying about their experiences in reviews?

This project follows CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology.
Steps followed in this project:
- **Business objective:** Analyze trends of availability, unavailability and price of properties all through the year, discuss how price can contribute to unavailability, factors that influence prices(does the number of bedrooms and guest included contribute to price), the best services in terms of property type and cancellation policy you can get at a price of $200 per day, the most popular Airbnb room type in the two cities, and what guests say about their experience with Airbnb.
- **Data Processing:** Applied certain data cleaning and wrangling techniques, handled missing data, impute where necessary, removed the outliers, and perform some text preprocessing.
- **Modeling:** Answer questions by using appropriate aggregrate method following statistical standards.
- **Evaluation:** Present the result of the analysis in form of tables and graphs.

### Prerequisites<a name="prerequisites"></a>
- Install anaconda to manage your data environment[here](https://www.anaconda.com/products/individual)
- Run conda -V on your terminal to confirm conda is installed and its in your path 
- To create conda environment with a specific python version run `conda create -n airbnb-env python=3.7`
- To activate the virtual environment run `conda activate airbnb-env`  or `source activate airbnb-env`
- Next, you can add your virtual environment to Jupyter by running: `python -m ipykernel install --user --name=airbnb-env`
- Check if its among the kernel list with `jupyter kernelspec list`
- conda install jupyter to install jupyter notebook
- Run `jupyter notebook` to start the interactive environment

You can check the requirements.txt file for the prerequisites
- Pandas (data manipulation and analysis)
- NumPy (scientific computing)
- Matplotlib (visualizations)
- Seaborn (visualizations)
- NLTK (Natural Language Toolkit for analysis of descriptions and reviews)
- Jupyter (interactive tool to run notebooks)

### Data<a name="data"></a>
There are three categories of datasets utilized in this project.
listing.csv, calendar.csv and reviews.csv

### Running the code<a name="running"></a>

There are three files:
- [`CaliforniaTexasAirbnb.ipynb`](http://localhost:8888/notebooks/CaliforniaTexasAirbnb.ipynb) 
The listing and calendar data files where employed for analysis in this notebook
The analysis of trends for availability, unavailability and price of properties all through the year, analysis of how price can contribute to unavailability, analysis showing how factors such as number of bedrooms and guest included contribute to prices, the best services in terms of property type and cancellation policy you can get at a specific price.
- [`AirbnbReviewSentimentAnalysis.ipynb`](http://localhost:8888/notebooks/Airbnb%20review%20sentiment%20analysis.ipynb)
The listing and review data files where employed for analysis in this notebook
Guests comments where labelled as positive, negative and neutal class using the review score ratings. The analysis for the most frequent words was performed

### Summary of Results<a name="results"></a>
- More expensive homestay?
  - For available Airbnb homes, the number of rental properties is slightly higher in the San-Francisco area than in Austin.
  - For unavailable Airbnb homes the average price for the Austin area is higher than the San-Francisco
- more costs incurred?
  - No. This is because the request for additional services might have an impact on price but does not always result in a high price.
- Better services for a price of $200?
  - Houses are more available at the rate of $200 in Austin than San-Francisco.
- more lenient city with the cancellation policy
  - Both cities but San-Francisco has the affordable price support for a higher proportion of 14 days grace period cancellation policy than Austin
- Popularity of room types
  - Entire homes or apartments are the most popular room types in both cities but it is more popular in Austin than San-Francisco.
- Experiences in reviews
  - Positive reviews supercedes other class of reviews
### Acknowledgements<a name="acknowledgements"></a>
-  [Kaggle](https://www.kaggle.com/aashirwad01/airbnb-analysis)
-  [Stackoverflow](https://stackoverflow.com/)
