# nosql-challenge
Module 12 Challenge - NoSQL

In this project, the main challenge is to import establishments data from a json format file into a MongoDB database. The json file contains a list of establishments in the United Kingdom and their relevant food hygiene ratings. The data is then updated using python in Jupyter Notebook and finally some analysis is performed.

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

In this step, I imported the establisments.json file into a MongoDB database "uk_food" by using a command line in Anaconda Prompt (I had to ensure that the dev environment was enabled first, and I was pointing to the relevant folder containing the establisments.json file). In Jupyter Notebook, I verified that the database had been created, and that the collection "establishments" was also there, assigning the establishments collection to a variable in preparation for use in the part 2 of the challenge.

Tools/Libraries I Imported:
- pymongo library: to enable interaction to MongoDB database
- pprint library: used to see output in a 'pretty print' for better readibility

My Files:
- Jupyter Notebook Python Script: NoSQL_setup_kt.ipynb
- JSON file: Resources/establishments.json


**Part 2: Update the Database**

In this section, I completed some changes to the data. Firstly, I added another restaurant to the "establishments" collection. Then I updated the "BusinessTypeID" for that new restaurant according to the other existing records in the database that contained BusinessType = "Restaurant/Cafe/Canteen". Any restaurants that were located in Dover were deleted from the database. Lastly, I updated the datatypes for longitude and latitude records from string to decimal numbers, and the RatingValue to integer numbers. Note. The RatingValue initally contained string values with text, these had to be changed to null values before changing all the values to integers.

Tools/Libraries I Imported:
- pymongo library: to enable interaction to MongoDB database
- pprint library: used to see output in a 'pretty print' for better readibility

My Files:
- Jupyter Notebook Python Script: NoSQL_setup_kt.ipynb
- JSON file: Resources/establishments.json


**Part 3: Exploratory Analysis**

In this final section, I used python libraries (pymongo, pprint and pandas) to perform analysis on the establishment data by performing queries, displaying the results in pretty print and then converting the results into Pandas DataFrames. The queries included the following:
1. Which establishments have a hygiene score equal to 20?
2. Which establishments in London have a RatingValue greater than or equal to 4?
3. What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
4. How many establisments in each Local Authority area have a hygiene score of 0?

Tools/Libraries I Imported:
- pymongo library: to enable interaction to MongoDB database
- pprint library: used to see output in a 'pretty print' for better readibility
- pandas library: for data manipulation and analysis

My Files:
- Jupyter Notebook Python Script: NoSQL_analysis_kt.ipynb 

## Getting Started
To open the files NoSQL_setup_kt.ipynb and NoSQL_analysis_kt.ipynb in Juypter Notebook:
  - Open Anaconda Prompt
  - Activate dev environment, type 'conda activate dev'
  - Navigate to the folder where repository is saved on local drive
  - Open Jupyter Notebook, type 'Jupyter Notebook'

To interact directly with MongoDB:
- Open MongoDBCompass (note. not required for the challenge, although can assist with gaining a better understanding of the data)
        
## Installing
Installed the following:
- PyMongo installation: after activating dev environment in Anaconda Prompt (see Getting Started above), type: "pip install pymongo" 
- MongoDB installation: go to website and follow instructions to download the MongoDB Community Server (https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-windows/)
