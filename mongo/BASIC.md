# List all Databases
 $ show dbs

# clear terminal
 $ cls

# Create a Database
 $ use database_name

# ----------------BASIC---------------------------
# insert
 # db.collection.insertOne({property1: 'A book', property2: 15.00})
  # Sample
   $ db.products.insertOne({name: 'A book', price: 15.00})

# List
 # db.collection.find()
 # Sample
   db.products.find()
   db.products.find().pretty()

# ----------------------------------------------------
# Find() method do not retrieve all data nor the whole array, but a cursor
# To get an array you must chain an array method
db.collection.find().toArray()

# Another way
db.collection.find().forEach(
    (document) => { printjson(document) }
)

db.collection.find().forEach( document => printjson(document) )

# Samples
db.passengers.find().forEach( passengerData => printjson(passengerData) )

# Drop Database
use databaseName
db.dropDatabase()

# Get rid of a collection
db.myCollection.drop()

# See status of the Database
db.stats()