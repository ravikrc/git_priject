# git_popularity_project

The Project aim is to show the popularity in % of github users in melbourne based on their followers,

In order to find the solution i needed the data, Initially i faced so many problems while scraping the data, as it is not allowing to scrap enough users, for that i needed to use selenium webdriver and scraped data and coded in python. 

I could able to get the following details of 1000 users from all the available pages of Melbourne github users:

1.user's link

2.users's name

3.users's follower's

4.users's star's

5.user's following

The data is stored  in userdetails.csv

But the aim of the project is to find popularity of the user based on their followers, for that i used mathematical function to display the percentage of the particular user.

The coding is done is jupyter notebook and stored in git_melbourne.ipynb

Steps followed to execute the code:

input:

The link of the user is pasted in colon:

df2 = df1.loc["the link of the user needed to be pasted here"]

we get the following output as:

The User is in the top 32.05128205128205 of Melbourne Github users based on followers


