# nonsql-challenge
MongoDB is a NoSQL database that is known for its flexibility, scalability, and ease of use. Unlike traditional relational databases that use tables and rows to store data, MongoDB stores data in a flexible, JSON-like format called BSON (Binary JSON).

## Create a new repository 'nonsql-challenge'
git clone into my local computer
Add setup notebooks and resources to the local repository
git add .
git commit -m "Add initial files"
git push origin main

## Import Database
Open Anaconda Prompt
Make sure it is under dev environment by running 'conda activate dev'
Run the 'mongoimport' command
The syntax is mongoimport --db uk_food --collection establishments --file "C:\Users\freya\BOOTCAMP\nonsql-challenge\Resources\establishments.json" --jsonArray
Open new Anaconda Prompt
Run 'mongod' to start the MongoDB Server under dev environment

## Database Setup
In the 'NoSQL_setup_starter.ipnynb' notebook, import the libraries you need: PyMongo and Pretty Print (pprint).
Create an instance of the Mongo Client.
Confirm that I created the database and loaded the data properly:
List the databases you have in MongoDB. Confirm that uk_food is listed.
List the collection(s) in the database to ensure that establishments is there.
Find and display one document in the establishments collection using find_one and display with pprint.
Assign the establishments collection to a variable to prepare the collection for use.
Insert a new business opened in Greenwich with its database.
Update the new restaurant with the BusinessTypeID.
Check how many documents contain the Dover Local Authority.
Rmove any establishments within the Dover Local Authority from the database.
Check the number of documents to ensure they were deleted.

## Database Analysis
In 'NoSQL_analysis_starter.ipynb' notebooj, I explored the database and convert into DataFrames by answering the questions listed in the notebook.
