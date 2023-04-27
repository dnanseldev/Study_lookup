# Only retrieving interested data
# Syntax 
# db.collection.find({}, {field: 1})

# Samples
db.passengers.find({}, {name: 1})

# To negate _id
# Must assign it to zero like _id: 0

# Sample
db.passengers.find({}, {name: 1, _id: 0})
db.passengers.find({}, {name: 1, _id: 0}).forEach( p => printjson(p) )

# Getting list of data, or child documents from a collection
# Arrays
db.passengers.findOne({name: 'Albert Twostone'}).hobbies

# Objects
db.flights.find({
    "status.description": "on-time"
})

db.flights.find({
   "status.details.responsable": "Dan Stonebuilt"
})