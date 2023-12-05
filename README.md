# INFO5002-Intro to Python for Information System 
# Final Project 
# OnlineMarketPlace 
# By Sirui Wei, Xingyan Huang, Peiyu Lin, Weizhou Zhou

This is an online trading platform where users can post items they want to sell or browse items that's posted by other users. 

#  Post New Items:
User can post his/her items by providing the category, name, description, price and picture informations when declaring a new item for sale on the market place. 
Category: Predefined categories [Toy, Furniture, Clothes]
Name: User defined 
Description: User defined 
Price: User defined 
Picture: User upload picture, default blank if user not provided a picture 

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
