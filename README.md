# nosql-challenge
Module 12 Challenge - NoSQL

In this project, the main challenge involved collecting data from websites by using web scraping. The two websites were:

- Mars News:
    - https://static.bc-edx.com/data/web/mars_news/index.html
    - I scraped information from a list of news articles
- Mars Weather:
    - https://static.bc-edx.com/data/web/mars_facts/temperature.html
    - I scraped weather information from a table. Then I performed some analysis on the scraped table data

Repository Contents:
- NoSQL_setup_kt.ipynb
- NoSQL_analysis_kt.ipynb
- Resources:
    - establishments.json
    
## Table of Contents

- [About](#about)
- [Getting Started](#getting_started)
- [Installing](#installing)

## About
**Part 1: Database and Jupyter Notebook Set Up**

Summary of what i did in this step

Tools/Libraries I Imported:
- splinter library: used for automating web browser actions
- bs4 library: Beautiful Soup, used for parsing websites and scraping specific data
- json library: to save the exported data in json format
- pathlib library: to create a file path to export the json file to

My Files:
- Jupyter Notebook Python Script: part_1_mars_news_kt.ipynb
- JSON file: Output/scraped_data_kt.json)


**Part 2: Update the Database**

Summary of what I did in this step

Tools/Libraries I Imported:
- splinter library: used for automating web browser actions
- bs4 library: Beautiful Soup, used for parsing websites and scraping specific data
- matplotlib.plplot module: from the matplotlib library, used to create various plots
- pandas library: for data manipulation and analysis

My Files:
- Jupyter Notebook Python Script: part_2_mars_weather_kt.ipynb
- csv file: Output/mars_temperature_data.csv


**Part 3: Exploratory Analysis**

Summary of what I did in this step

Tools/Libraries I Imported:
- xxx library: used for automating web browser actions

My Files:
- Jupyter Notebook Python Script:   

## Getting Started
To open the files NoSQL_setup_kt.ipynb and NoSQL_analysis_kt.ipynb in Juypter Notebook:
  - Open Anaconda Prompt
  - Activate dev environment, type 'conda activate dev'
  - Navigate to the folder where repository is saved on local drive
  - Open Jupyter Notebook, type 'Jupyter Notebook'

To open MongoDB:
- Open MongoDBCompass
        
## Installing
Installed the following:
- PyMongo installation: after activating dev environment in Anaconda Prompt (see Getting Started above), type: "pip install pymongo" 
- MongoDB installation: go to website and follow instructions to download the MongoDB Community Server (https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-windows/)
