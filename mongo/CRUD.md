# Create
insertOne(data, options)
insertMany(data, options)
# -------------------------------------
# Read
find(filter, options)
findOne(filter, options)
# -------------------------------------
# Update
updateOne(filter,data, options)
updateMany(filter,data, options)
replaceOne(filter,data, options)

# samples
 db.flights.updateOne({
    {distance: 12000}
    ,{$set: {marker: "delete"}}
 })

 db.flights.updateMany(
    {}
    ,{$set: {marker: "toDelete"}}
 )
# -------------------------------------
# Delete
deleteOne(filter, options)
deleteMany(filter, options)

db.flights.deleteMany(
    {marker: "toDelete"}
)
