# OnlineMarketPlace | Django

This is an online trading platform where users can post items they want to sell or browse items that's posted by other users. 

## Author
This project is completed by Sirui Wei, Xingyan Huang, Peiyu Lin, Weizhou Zhou

# Project Envrionment Setup 
Open the proejct with VSCode, make sure you have latest python installed on your computer 

## Setting virtual environment
Open a new Terminal by clicking NewTerminal button on top of you VSCode Terminal section 

Then type in: 
#### python3 -m venv env

Here "env" is the name of your virtual environment
env is an isolated virtual environment just for this project where you can install python packages such as Django 
Upon creating a new virual environment you should be able to see a new folder called env

## Activate virutal environment 
In the same terminal type in:
#### source env/bin/activate 
You should be able to see an (env)/ at the beginning of your terminal directory on your terminal 

## Install django and pillow 
In the same terminal type in:
#### pip install django

After finishing django package then type in:
#### pip install pillow 

## Finish 
When finishing installing these two packages your virtual environment is now ready to run this website! 

# Run the website 
Open a new terminal, and make sure your new terminal path is in the same directory as OnlinMarketPlace-django
If your are not sure, right click on the (OnlineMarketPlace-django) folder beneath (env) folder, and select "Open in Integrated Terminal"
Then you should be on track, and type in: 
#### python manage.py runserver 

You should be able to see the following messages: 

#### System check identified no issues (0 silenced) <br />
#### December 06, 2023 - 22:41:29 <br />
#### Django version 4.2.5, using settings 'myproject.settings' <br />
#### Starting development server at http://127.0.0.1:8000/ <br />
#### Quit the server with CONTROL-C. <br />
 
Copy the server address  http://127.0.0.1:8000/ and paste it into your system browser <br />
You should be able to see the fron page of the server with Sign up and Login on top right 

# Become the super user of the website! 
In order to manage the website and access the database of the site, your should register as SuperUser, or Admin <br />
However you can't do it directly on the website
In your VSCode, open a new terminal and type in:
#### python manage.py createsuperuser 
Then you will be asked to input your user name, which I recommend using admin <br />
Then you will be asked to input and confirm your password. You won't be able to see what you typed in the password <br />
Just keep typing and press enter when you are done. Do the same for Confirm Your Password too 
### Login as admin 
On the website you can login with your super user credentials, however it will just perform as a normal user <br />
In order to access admin site, on the url of your brower type in: 
#### http://127.0.0.1:8000/admin 
Login here with your super user credentials and you should be able to access the database of the website <br />
In here you can manage the website users, their items and the conversations between users

# Sign Up, Login and Logout
When you luanch the website for the first time, you should be able to see a sign up button on the top right <br />
Click on sign up and enter your username, which you will be using for logging in, your email, and your password <br />
After signing up you will be redirected to sign in page and sign in with the credentials you just provided. <br />

In terms of log out, you need to go to the admin site and log out from there <br /> 
There is no logout button on the website page <br />

# Post New Items:
After signing up, login with your credentials <br />
You can post items by providing the category, name, description, price and picture informations when declaring a new item for sale on the market place. <br />
Category: Predefined categories [Toy, Furniture, Clothes]  <br />
Name: User defined  <br />
Description: User defined  <br />
Price: User defined  <br />
Picture: User upload picture, default blank if user not provided a picture  <br />

# Browse items: 
User can browse items online using search function. The search function find product if either name or description matched user input in the search bracket 
Category filter is also implemented, user can browse items based on categories

# Conversation with other users:
For each product posted on the market place the user is able to contact the seller directly thorugh Contact Seller button. 
The user is able to send a message to seller and the message will appear in the Inbox on the page of the seller. 
Each user has an inbox for receiving and sending messages, all previous conversation is saved in the Inbox for future references. 

# Dashboard: 
Every user has a dashboard where he/she can manage the products posted, and the user can change the price, name and description of his/her products posted. 
There is also a IS_SOLD checkbox to notify other users whether this specific product is sold. 
If the IS_SOLD is checked for a product, it won't be shown on the trading homepage anymore 
