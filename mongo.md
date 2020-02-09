# Mongo
* `mongo -u <username> -p <pass> --authenticationDatabase <usually admin>`: Login with mongo shell.
* `mongoimport --db <dbname> --collection <collection name> <path to json> <auth see above>`: Import collection using mongo shell.

* `db.collection.getIndexes()`:
* `db.collection.createIndex( { key_name: 1 }, { unique: true } )`:


See also: 
* https://api.mongodb.com/python/current/tutorial.html
