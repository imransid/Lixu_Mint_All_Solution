# MongoDB


## cls

> cls is used for clear all screen

## show dbs

> To view all databases

## use mycustomers

> create and switch database

## createUser({})

> make a user

db.createUser({
    user: "brad",
    pwd: "1234",
    roles: ["readWrite", "dbAdmin"]
});

## db.createCollection(name, options)

> collection is samilar table to relation database

## show collections

> To view total collection

## db.name.insert({})

> To insert vale collection

## db.customers.find()

> To Show all store data.

## db.customers.find().pretty();

> To show collection more better

## db.customers.update({id: 000},{first_name: "Imran"})

> To Update value collection 

## db.customers.update({id: 000},{$set : {gender : "male"}})

> $set use to unchanged other value fixed those key what we want to change

## db.customers.update({id: 000},{$unset: {age: 21}})

> If the field does not exist, then $unset does nothing (i.e. no operation).

## db.customers.update({first_name : "Hafiz"},{first_name : "Hafiz", age : 29}, {upsert : true});

> upsert use if not found it insert data

## db.customers.update({first_name : "Nisan"},{$rename : {"gender" : "sex"}})

> $rename is use for rename row or key name

## db.customers.remove({first_name : "Nisan"})

> remove is use delete row

## db.customers.remove({first_name : "Nisan"},{jsutOne : true})

> Delete first One find not all

## db.customers.find({first_name : "Imran"}).pretty();

> find first_name is Imran

## db.customers.find({$or: [ {first_name : "Imran"}, {first_name : "Jisan"} ]})

> find Imran name and Jisan what is avaliable.

## db.customers.find({age: {$lt : 40}}).pretty();

> less then 40 age all show

## db.customers.find({"address.city": "Barisal"})

> It will find address nesder city Barisal :) 

## db.customers.find().sort({last_name : 1})

> it will assending data A-Z

## db.customers.find().sort({last_name : 1})

> it will reversr A-Z view(Z-A)

## db.customers.find().count()

> total row..

## db.customers.find({age : 29}).count()

> age row available row total

## db.customers.find().limit(3)

> first 3 row show

## db.customers.find().limit(2).sort({last_name:1})

> last name sort first 2

## db.customers.find().forEach(function(doc){ print("Customer Name : " + dec.first_name)});