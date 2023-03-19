# nodejs-day5
nodejs-day5  

mongodb commands


show dbs  - shows all databases
show collections - show collections

use <name of the db>  to create a dataabse

db.orderdetails.insertOne({item:"pizza",price:1299})  - inserting a document in a orderdetails collection
db.orderdetails.insert({item:"burger",price:299})  
db.orderdetails.insertMany([{item:"momos",price:199},{item:"dosa",price:70},{item:"biriyani",price:499}])

db.orderdetails.find()
db.orderdetails.find({}) 
db.orderdetails.findOne({})
 db.orderdetails.find({price:299})
db.orderdetails.find({_id:ObjectId("6415eda35ac415c8b4fbbcd8")})
db.orderdetails.find().pretty()

db.orderdetails.update({_id:ObjectId("6415eda35ac415c8b4fbbcd8")},{$set:{restaurant:"mcdonalds"}}
db.orderdetails.updateOne({_id:ObjectId("6415eda35ac415c8b4fbbcd8")},{$set:{restaurant:"mcdonalds"}}





 db.orderdetails.remove({_id:ObjectId("6415eda35ac415c8b4fbbcd8")})- removes the document from collection

db.fooddetails.drop() -removes the collections from db 


https://www.mongodb.com/docs/ -- mongodb documentation

npm install express mongodb nodemon





