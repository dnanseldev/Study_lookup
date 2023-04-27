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