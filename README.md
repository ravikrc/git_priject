# git_popularity_project

# steps followed to run the project

# Installing Anaconda to use the jupyter notebook:

## method 1: running the project from scratch by scraping data

To the run the code we need jupyter notebook, to get the jupyter notebook, we need to install anaconda, 

## Here are the instructions to follow to install anaconda on windows:

https://docs.anaconda.com/anaconda/install/windows/

##  Here are the instructions to follow to install anaconda on mac:

https://docs.anaconda.com/anaconda/install/mac-os/

After installing the Anaconda, you will see a jupyter notebook, press launch tab , it will display the locations of your computer.

Before running the code TYPE pip install selenium in command prompt, that will install selenium on to your computer.

Now download files  git_melbourne.ipynb, web_scrap.ipynb. from my repo.

Open web_scrap.ipynb, from jupyter notebook, you will see the prewritten code to execute, now go to google chromebrowser and type chromedriver for selenium, install latest chromedriver as per your computer requirements, here is the location http://chromedriver.chromium.org/downloads, store this chromedriver in any of the location and copy that path and paste it in both the lines of code in colons where is mention #set chromedriver path 

Exapmle:

#set chromedriver path

sub_driver = webdriver.Chrome(options=options, executable_path=r'\Users\ravichandrachilupuri\Downloads\chromedriver')

#set chromedriver path

driver = webdriver.Chrome(options=options, executable_path=r'\Users\ravichandrachilupuri\Downloads\chromedriver')

After completing the steps, press run tab, it will start scraping the data. the data will be scraped and stored in a file named with user_details and that will be stored in the same location where the scraping data is done(ex: user details.csv)

Now open the git_melbourne.ipynb, which is in same location copy and paste the file name in second line of the code:

ex:
read the userdetails file
df = pd.read_csv('user_details.csv')

At the end copy and paste the desired link of the user in colons, next to df1.loc and run the code:

Example:

input:

df2 = df1.loc["https://github.com/JakeLin","Popularity_F"]

print('The User is in the top',df2,'of Melbourne Github users based on followers')

output:

The User is in the top 32.05128205128205 of Melbourne Github users based on followers


# Method 2: without scraping the data:

Download the user_details.csv and store in the same location where you stored git_melbourne.ipynb

Now open the git_melbourne.ipynb, which is in same location copy and paste the file name in second line of the code:

ex:
#read the userdetails file
df = pd.read_csv('user_details.csv')

At the end copy and paste the desired link of the user in colons, next to df1.loc and run the code:

Example:

input:

df2 = df1.loc["https://github.com/JakeLin","Popularity_F"]

print('The User is in the top',df2,'of Melbourne Github users based on followers')


The Project aim is to show the popularity in % of github users in melbourne based on their followers,

In order to find the solution i needed the data, Initially i faced so many problems while scraping the data, as it is not allowing to scrap enough users, for that i needed to use selenium webdriver and scraped data and coded in python. 

The webscraping coding is done is following file:

web_scrap.ipynb

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


