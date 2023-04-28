# Greater than
 db.collection.find({
    field: {$gt: parameter}
 })

# Sample
db.flights.find({
    distance: {$gt: 1000}
})

# -------------------
# Lesser than
 db.collection.find({
    field: {$lt: parameter}
 })

# Sample
db.flights.find({
    distance: {$lt: 1000}
})
