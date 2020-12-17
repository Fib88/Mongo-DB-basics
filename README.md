# Mongo-DB-basics

First look at Mongo DB database. I'm updating the readme as I go trough the steps.

For installation I followed the steps at [Mongo DB official website](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/).

***To start MongoDB run:***   
*sudo systemctl start mongod*

***To check if MongoDB is running use:***   
*sudo systemctl status mongod* 

***To enter the Mongo DB shell enter:***   
*Mongo*

*******
### Creating a DB with Mongo:   
***commands:***   
- *show databases* or *show dbs*
- *use name of database*-> creates or selects a DB   
- *show dbs* ->list of all databases created
- *db* -> currently selected db
-*show collections* -> lists collections in db

*******



### C - Inserting data with Mongo  
<u>insert:</u>   
 db.nameofcollection.insert({name: "Fib", age: 100, coolGuy: True})   
 <u>showinserteddata:</u>   
 db.nameofcollection.find()
*******
### R - Finding data with Mongo
*******
### U - Updating data with Mongo
*******
### D- Deleting with Mongo

