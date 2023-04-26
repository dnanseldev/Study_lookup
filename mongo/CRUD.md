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
 # Obs update command. There are another update command that overwright the previus data/objetc that is:
 # db.collection.update({filter: parameter}, {new object})
 # sample:
 db.flights.update({
    id: _id: ObjectId("64494c992ef1a6b39281c8c2")
    ,{delayed: false}
 })

 # The delayed field will replace all of those previeus fields keeping only _id and the new one, delayed.
# -------------------------------------
# Delete
deleteOne(filter, options)
deleteMany(filter, options)

db.flights.deleteMany(
    {marker: "toDelete"}
)
