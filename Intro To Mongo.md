# Mongo
Basic MongoDB commands

## Setup  
Type one of the following commands in terminal:  
- mongo to access local databases  
- mongo "<url"> --username <username> to access databases in mongo atlas cluster. In this case you will be prompted to enter password.  
  
 ## Some simple commands to start with:  
 - show dbs - to show available databases  
 - use <dbname> - to use (or create) a database named <dbname>  
 - show collections - to show collections in current database  
 - db.<collection-name>.insert({"field name 1":"field value 1", "field name 2":"field value 2", ..., "field name x":"field value x"})  
 - db.<collection-name>.insert([<object1>, <object2>, ..., <objectn>]}  
 - db.<collection-name>.find() - to obtain all objects in collection  
 - db.<collection-name>.find().pretty() - to obtain result in readable format  
 - db.<collection-name>.find().sort() - to obtain result in sorted order  
 - db.<collection-name>.findOne() - to obtain first object     
 - db.<collection-name>.find({"field name":"field value"}) - to find objects that satisfy given criteria  
 - db.<collection-name>.find({ $and: [ {<key1>:<value1>}, { <key2>:<value2>} ] }) - object satisfies both criterias
 - db.<collection-name>.find({ $or: [ {<key1>:<value1>}, { <key2>:<value2>} ] }) - object satisfies either criteria  
 - db.<collection-name>.find({ $not: [{<key1>:<value1>}]}) - object does not satisfy criteria  
 - db.<collection-name>.update({<key1>:<value1>},{$set:{<new key>:<new value>}},{multi:true}) - to update  
 - db.<collection-name>.updateOne({<key1>:<value1>},{$set:{<new key>:<new value>}},{multi:true})  
 - db.<collection-name>.remove({<key1>:<value1>}) - to delete objects satisfying criteria  
 - db.<collection-name>.remove({<key1>:<value1>}, 1) - to delete one object that satisfies criteria  
 - db.dropDatabase() - to drop current database  
 - db.<collection-name>.drop() - to drop a collection  
 
 
 
 
