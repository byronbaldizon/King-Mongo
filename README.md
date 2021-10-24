

# KING-MONGO
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
    
    
 


   
    
    
    
