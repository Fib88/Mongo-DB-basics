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
  *db.nameofcollection.insert({name: "Fib", age: 100, coolGuy: True})* -> Inserts data into collection   
*******
### R - Finding data with Mongo      
 *db.nameofcollection.find()* -> reads data from collection   
 *db.nameofcollection.find({age:100})* -> filters data from collection where age:100 
 
 For specifying filter conditions more check out the docs at [query conditions](https://docs.mongodb.com/manual/tutorial/query-documents/#read-operations-query-argument)
 
*******
### U - Updating data with Mongo
*db.nameofcollection.updateOne({name:"Fib"}, {$set{color:green}})* ->updates one entry where name: Fib, second argument with *$set* operator updates the value of color to green
*******
### D- Deleting with Mongo
*db.nameofcollection.deleteOne({age:25})* ->deletes one entry where age:25   
*db.nameofcollection.deleteMany({})* -> deletes entire collection
