# There are 2 aproachs

# --> embedded

# --> references

{
    _id: ObjectId("644ab4ac52d6d5c947226aa1"),
    name: 'Daniel Stonebuilt',
    age: 38,
    diseaseSumary: 'sum-pac-dis-01'
}

{ _id: 'sum-pac-dis-01', diseases: [ 'cold', 'broken leg' ] }

# ------Approach 1

 var dsid = db.patients.findOne({name: "Daniel Stonebuilt"})
 db.diseaseSumaries.findOne({_id: dsid})

# ---------Joining with $lookup operator

# -----------Samples

# Customers

{
    userName: 'Max',
    favBooks: ['id1', 'id2']
}

# Books

{
   _id: 'id1',
   name: 'Lord of the Rings 1'
}

# --------------------

customers.aggregate([
    {
        $lookup: {
            from: "books",
            localField: "favBooks",
            foreignField: "_id"
            as: "favBookData"
        }
    }
])

# Obs: Must install the aggregation framework
