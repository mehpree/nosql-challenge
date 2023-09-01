# NoSQL Database and Data Analysis Project

## Introduction

Welcome to the NoSQL Database and Data Analysis project! In this assignment, I have worked on evaluating food hygiene ratings data provided by the UK Food Standards Agency. The goal of this project is to assist the editors of a food magazine, Eat Safe, Love, in analyzing the ratings data to help their journalists and food critics decide where to focus future articles.

## Part 1: Database and Jupyter Notebook Setup

In this section, I have set up the NoSQL database and prepared the Jupyter Notebook for data analysis. Here are the key steps I've followed:

1.  **Data Import:** I imported the data provided in the `establishments.json` file into a MongoDB database named `uk_food` and a collection named `establishments`. The data import was done via the Terminal, and I have documented the import command in a Markdown cell within the notebook.
    
2.  **Library Imports:** Within the Jupyter Notebook, I imported the necessary Python libraries, including PyMongo for database interaction and Pretty Print (pprint) for displaying data.
    
3.  **MongoDB Client:** I created an instance of the MongoDB client to connect to the database.
    
4.  **Data Validation:** I confirmed the successful creation of the database and the `establishments` collection by listing the available databases and collections. Additionally, I retrieved and displayed one document from the `establishments` collection using `find_one`.
    
5.  **Variable Assignment:** I assigned the `establishments` collection to a variable for further analysis.
    

## Part 2: Update the Database

In this section, I made requested modifications to the database before performing queries or analysis. The following changes were made to the `establishments` collection:

1.  **Addition of New Restaurant:** I added a new halal restaurant in Greenwich to the database as per the magazine's request.
    
2.  **BusinessTypeID Query:** I found the BusinessTypeID for "Restaurant/Cafe/Canteen" and returned only the BusinessTypeID and BusinessType fields.
    
3.  **Update New Restaurant:** I updated the information of the new restaurant with the BusinessTypeID found in the previous step.
    
4.  **Deletion of Dover Establishments:** I identified and removed establishments within the Dover Local Authority from the database.
    
5.  **Data Type Conversion:** I used `update_many` to convert latitude and longitude to decimal numbers and also to convert RatingValue to integer numbers.
    

## Part 3: Exploratory Analysis

In this section, I performed an exploratory analysis of the dataset to answer specific questions posed by Eat Safe, Love. Each question was addressed using MongoDB queries, and the results were presented in a structured manner. Here are the questions I explored:

1.  **Establishments with Hygiene Score 20:** Identified establishments with a hygiene score equal to 20.
    
2.  **High-Rated Establishments in London:** Found establishments in London with a RatingValue greater than or equal to 4.
    
3.  **Top 5 Establishments with RatingValue 5:** Determined the top 5 establishments with a RatingValue of 5, sorted by the lowest hygiene score and nearest to the new restaurant "Penang Flavours."
    
4.  **Local Authorities with Hygiene Score 0:** Counted establishments in each Local Authority area with a hygiene score of 0, sorted from highest to lowest. Displayed the top ten local authority areas.
    

This project showcases my skills in working with NoSQL databases, data analysis, and querying MongoDB to derive valuable insights from real-world data. It provides Eat Safe, Love with the information needed to make informed decisions about future articles and restaurant recommendations. Enjoy exploring the world of food hygiene ratings!

### References
[UK Food Standards Agency](https://www.food.gov.uk/) (2022). UK food hygiene rating data [API](https://ratings.food.gov.uk/open-data/en-GB). Contains public sector information licensed under the [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).
Accessed Sept 9, 2022 and Sept 12, 2022 with the establishment settings as follows: longitude=51.5072, latitude=-0.1276, maxdistancelimit=4567, pagesize=10000, sortoptionkey=distance, pagenumber=(1,2,3,4,5,6,7,8).

#### © 2023 edX Boot Camps LLC




