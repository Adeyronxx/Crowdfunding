# Crowdfunding-ETL
This is a project for Independent Funding, a crowdfunding platform which helps generate funding for independent projects and ventures. Independent funding received a new dataset that contains information about the backers who’ve pledged to the live projects. 

# Goal of the project.
1. Extract the information we need to perform an analysis.
2. Transform and Clean the data to make our analysis process easier.

# Resources

* Jupyter Notebook
* Quick DBD
* PgAdmin
* CSV file (backer_info.csv)

# Analysis

# Result

To conduct our Analysis, we first had to do 3 things;

1. First we imported our csv file and extracted the backers information

<img width="827" alt="Screenshot 2022-11-05 at 6 31 14 PM" src="https://user-images.githubusercontent.com/109445468/200147167-a58afef2-977c-49f8-b786-54e042e40dbd.png">

Next, we created a new DataFrame to store our information in 4 columns; (backer_id, cf_id, name and email address)

<img width="827" alt="Screenshot 2022-11-05 at 6 33 06 PM" src="https://user-images.githubusercontent.com/109445468/200147221-d6b90a0b-1358-40ff-8e97-c1ac7437dd77.png">

2. To transform and clean the data we further added a first and last name column and eliminated the 'name' column and exported this into a new csv file.

<img width="814" alt="Screenshot 2022-11-05 at 6 33 31 PM" src="https://user-images.githubusercontent.com/109445468/200147275-e601b672-e08b-42a1-90e4-8148d4feb89a.png">


3.  Load the data into a database

Here, we first created a table schema to show the relationship between all the data available to us

![crowdfunding_db_relationships](https://user-images.githubusercontent.com/109445468/200147424-1a72f716-43ef-4072-8333-c7f7570f59a4.png)

Next, we created a database and imported all our data

<img width="625" alt="Screenshot 2022-11-05 at 6 34 55 PM" src="https://user-images.githubusercontent.com/109445468/200147449-bfe1c206-ae3a-4401-88fd-c53327734816.png">

4. Lastly, we had to determine the amount needed to reach the funding goals on the live campaigns.

<img width="624" alt="Screenshot 2022-11-05 at 7 02 28 PM" src="https://user-images.githubusercontent.com/109445468/200147793-3419456c-9b52-4da2-828f-a90bd3c0eb1a.png">


# Summary

In conclusion, we are clearly able to see the names and email information for the backers of each campaign. This will make reaching out to them and informing them of the amount remaining to reach the pledged goal easier.
