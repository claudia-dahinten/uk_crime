# uk_crime

As part of the Immersive Data Science course at General Assembly students receive a 3 month free Tableau trial. Since I enjoy visualisations and Tableau seems to appear ubiquitously on job adverts, I thought I'd spend some time creating a Dashboard.

I recently had something stolen in London, and through this came across a crime database managed by the police. I decided to use that as my guinea pig.

<h3/>GETTING THE DATA<h3/> <br/>
The data was relatively straight forward to obtain. It is saved in a database on the data.police.uk website. Every month of every year is saved in a separate folder and each folder has a csv file that corresponds to the different police departments. Due to the clean structure, I was able to write some lines of code to extract each csv and concatenate them into a dataframe.

DATA CLEANING<br/>
There was really not much I needed to clean as it's a very well maintained dataset. I did drop a few rows and columns that were redundant or had many missing values. I also created a new column to group crime types into larger categories.

EDA<br/>
It was fun to explore the data and I made the following findings:
- Between 2017 and 2019 there have been over 19 million reported crimes in the UK
- Unsurprisingly most crimes (3 million) are reported to the London Metropolitan Police
- If you live in London you want to stay away from Westminster, Camden and Tower Hamlets if you want to stay safe
- Interestingly the council (LSOA) with the most crime in the UK is Birmingham
- The majority of crimes occur near Supermarkets, Parking Areas and Shopping Areas
- Violent and sexual crimes are the highest reported crimes
- Crime appears to be seasonal as it increases during the summer in each year. There is also a big drop in December and subsequent increase in January

VISUALISATION<br/>
Following on from my initial analysis in Jupyter Notebook I created Dashboard in Tableau which can be viewed here: https://tinyurl.com/t5oduw9
In particular I was interested in:
- Creating a Dashboard to visualise the above on one page
- Showing the hotspots for crimes in a map
- Creating more interactivity for the user

CHALLENGES<br/>
- The main challenge in working with this dataset was the size. 3GB or 19 million rows is a lot for my computer to handle! Jupyter notebook reacts quite well to it, but Taleau struggled a little but more.
- Even though the dataset is large, there was limited information on each of the crimes. I would have liked to explore further information, such as demographics, day of the week, time of day etc.
- It was challenging to decide how to structure the Dashboard as I was unfamiliar with the Tableau functionality and best practices for creating dashboards. A lot of my time was spent on formatting.
