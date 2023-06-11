db.getCollection("Movies").find({})
db.getCollection("Movies").find({"year":2012})
db.getCollection("Movies").find({"year":{$gt:2012}})
db.getCollection("Movies").find({"merits.budget":{$gt:50}})
db.getCollection("Movies").find({"technical.runningTime":{$gt:105}})
db.getCollection("Movies").find({"technical.language":"English"})
db.getCollection("Movies").find({"year":{$gte:2010,$lte:2013}})
db.getCollection("Movies").find({"technical.runningTime":{$gte:100,$lte:110}})
db.getCollection("Movies").find({"cast":"Jennifer Aniston"})
db.getCollection("Movies").find({"year":{$lt:2012}},{"name":1, "_id":0})
db.getCollection("Movies").find({"merits.boxOffice":{$gt:500}},{"merits.boxOffice":1,"name":1, "_id":0})
db.getCollection("Movies").find({"year":{$in:[2010,2011,2012]}})



