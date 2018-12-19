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

>> $rename is use for rename row or key name

## db.customers.remove({first_name : "Nisan"})

>> remove is use delete row