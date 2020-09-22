# Mongo
* `mongo -u <username> -p <pass> --authenticationDatabase <usually admin>`: Login with mongo shell.
* `mongoimport --db <dbname> --collection <collection name> <path to json> <auth see above>`: Import collection using mongo shell.
* `mongodump --host mongodb.example.com --port 27017 --username user --password "pass" --out /backup/dir`

* `db.collection.getIndexes()`:
* `db.collection.createIndex( { key_name: 1 }, { unique: true } )`:

* connection string: mongodb://[username:password@]host1[:port1][,...hostN[:portN]][/[defaultauthdb][?options]] (see https://docs.mongodb.com/manual/reference/connection-string/)


See also: 
* https://api.mongodb.com/python/current/tutorial.html
