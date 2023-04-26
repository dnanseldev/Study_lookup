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