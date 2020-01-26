# uk_crime

As part of the Immersive Data Science course at General Assembly students receive a 3 months free Tableau trial. Since I enjoy visulisations and it seems ubiquitous on job ads, I thought I'd spend some time creating a dashboard.

I recently had something stolen in London, and came across the database by the police on crime data, so I decided to use that s my guinea pig.

GETTING THE DATA . 
The data was relatively straight forward to obtain. It is saved in a database on the website data.police.uk website. Every month of every year is saved in a separate folder and each folder has a csv file that corresponds to the differen police departments. Due to the clean structure, I was able to write some lines of code to extract the differenct csvs and concatenate them into a dataframe.

DATA CLEANING<br/>
There was really not much I needed to clean as it's a very well mainted dataset. I did drop a few rows and columns that were redundant or had many null values and created a new column to group crime types into categories.

EDA
It was fun to explore the data and I made the following findings:
- Between 2017 and 2019 there have been over 19 million reported crimes in the UK
- Unsurprisingly most crimes (3 million) are reported to the London Metropolitan Police
- If you live in London you want to stay away from Westminster, Camden and Tower Hamlets if you wants to stay safe
- Interestingly the council (LSOA) with the most crime in the UK is Birmingham
- The majority of crimes occur near Supermarkets, Parking Areas and Shopping Areas
- Violent and sexual crimes are the highest reported crimes
- Crime appears to be seasonal as they increase during the summer in each year, there is also a big drop in December and subsequent increase in January

VISUALISATION
Following on from my initial analysis in Jupyter Notebook I created Dashboard in Tableau which can be viewed here: https://tinyurl.com/t5oduw9
In particular I was interested in:
- Creating a Dashboard to visualise the above on one page
- Showing the hotspots for crimes in a map
- Creating more interactivity for the user

CHALLENGES
- The main challenge in working with this dataset was the size. Jupyter notebook reacts quite well to it, but Taleau struggled a little but more
- Even though the dataset it large, there was limited information on each of the crimes. I would have liked to explore further information, such as demographics, day of the week, time of day
- It was challenging to decide how to structure the Dashboard as I was unfamiliar with the Tableau functionality and best practices for creating dashboards.
