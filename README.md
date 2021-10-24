# KING-MONGO
## MongoDB install
+ Go to https://www.mongodb.com/es
![MONGO](https://i.postimg.cc/g07BZyyL/mongodb-1.png)
+ Click on *Software*
![MONGO](https://i.postimg.cc/NjfNCCpr/mongodb-2.png)
+ Select community server
![MONGO](https://i.postimg.cc/6qrHgDkC/mongodb-3.png)
+ Click on DOWNLOAD button and run the .msi installer
## mongosh install
+ Go to https://docs.mongodb.com/mongodb-shell/install/
![MONGOSH](https://i.postimg.cc/HstZ214g/mongosh-1.png)
+ Scroll down to Open the MongoDB Download Center and click on this link.
+ Follow instructions and complete the installation.
![MONGOSH](https://i.postimg.cc/1RwY8q84/mongosh-2.png)
+ Fill the form with the information and press the Download button
![MONGOSH](https://i.postimg.cc/tCbvW46k/mongosh-3.png)
+ Open to Windows Explorer
+ Go to Program Files and look for MongoDB file
+ Dive into the file and look for bin file
+ Select a copy the path to this file
![MONGOSH](https://i.postimg.cc/9XsQBGRD/mongosh-path.png)
+ Go to search field and write *environmental variables* (*variables de entorno*)
+ Select *edit system variables*
![MONGOSH](https://i.postimg.cc/K8tXyT8s/variables-de-entorno.png)
+ Click on new
![MONGOSH](https://i.postimg.cc/pLSBkcHw/path-3.png)
+ Paste the url to bin file
![MONGOSH](https://i.postimg.cc/HL79N0WV/path-4.png)
+ Click to accept
## Install MongoDB for VS Code extension
![MONGOSH](https://i.postimg.cc/g26Pg5hR/mongo-vs-code.png)



## Utilities
### Clear screen
    cls
### Show current database
    db
### Show all databases
    show dbs
### Get help
    help
### Shows a list of methods of *db* command
    db.help()
## DB Creation
### Creation of database: (no database will be created until a data is inserted)
    use <database name>
### Creation of collection in database: (database will be created)    
    db.<name-of-collection>.insert(<javascript-object>)
### Displaying collection of current database
    show collections
### Delete current database
    db.dropDatabase()
### Create a collection in current database
    db.createCollection("<name-of-collection>")
### Create a collection in current database (2).  MonogoDB creates a collection when a data is inserted.
    db.<name-of-collection-to-be-created>.insert()
### Delete a collection of current database
    db.<name-of-collection>.drop()
### Show all data stored in collection
    db.<name-of-collection>.find()
### Show all data stored in collection in a nice format
    db.<name-of-collection>.find().pretty()    
### Insert many documents
    db.<name-of-collection>.insert([{ <document-1-json-formatted> },{ object-2-json-formatted },...])
### Look for documents according to a key
    db.<name-of-collection>.find({ "key":"value" })    
### Look for documents according to multiple keys
    db.<name-of-collection>.find({ "key-1":"value-1" },{ "key-2":"value-2" })    
### Look for the first document according to a key
    db.<name-of-collection>.findOne({ "key":"value" })   
    
### Look for documents according to key but display selected keys in the result
    db.<name-of-collection>.find({ "key":"value" },{ "key-to-be-excluded":0,"key-to-be-included":1 })  
### Limit the number of results
    db.<name-of-collection>.find({ "key":"value" }).limit(number-of-results)
### Number of documents in a collection
    db.<name-of-collection>.count()
### Using functions with database data
#### Use of *forEach()* function
    db.<name-of-collection>.find().forEach(el=>print(el.<key>))
## UPDATE a document
### Update document (with overwriting)
    db.<name-of-collection>.update({"key":"value" <to find>},{"key":"value" <to replace>})
### Adding key to a document
    db.<name-of-collection>.update({"key":"value" <to find>},{$set{"key":"value" <to add>}})
### Adding new key with *upsert* (no overwrite)


    
    
 


   
    
    
    
