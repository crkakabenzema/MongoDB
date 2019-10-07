# MongoDB
The following content is review notes about MongoDB for MongoDB learners and developers. 

1. Operation difference between mongodb and sql:
下表列出了 RDBMS 与 MongoDB 对应的术语：
RDBMS 	MongoDB
数据库 	数据库
表格 	   集合
行 	    文档
列 	    字段
表联合 	嵌入文档
主键 	主键 (MongoDB 提供了 key 为 _id )

MongoDB 与 RDBMS Where 语句比较：
如果你熟悉常规的 SQL 数据，通过下表可以更好的理解 MongoDB 的条件语句查询：
操作 	   格式 	               范例 	                                         RDBMS中的类似语句
等于 	   {<key>:<value>} 	        db.col.find({"by":"菜鸟教程"}).pretty() 	   where by = '菜鸟教程'
小于 	   {<key>:{$lt:<value>}} 	db.col.find({"likes":{$lt:50}}).pretty() 	    where likes < 50
小于或等于 {<key>:{$lte:<value>}} 	db.col.find({"likes":{$lte:50}}).pretty() 	where likes <= 50
大于 	   {<key>:{$gt:<value>}} 	db.col.find({"likes":{$gt:50}}).pretty() 	    where likes > 50
大于或等于 {<key>:{$gte:<value>}} 	db.col.find({"likes":{$gte:50}}).pretty() 	where likes >= 50
不等于 	   {<key>:{$ne:<value>}} 	db.col.find({"likes":{$ne:50}}).pretty()  	where likes != 50

