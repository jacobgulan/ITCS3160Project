
## <b>Introduction</b>

The popularity of food delivery services has proliferated over the past few years with the pandemic lending hand to its rise. It’s expected that, even as life normalizes, the daily use of food delivery services will remain. Students are one of the main consumers of food delivery services. To ensure safety and health, some universities are considering devising their own campus delivery system.

## <b>Description</b>

Using a test database from “Team Mavericks,” our group plans to enhance this database to include a rating system for delivery drivers and restaurants. Our group will also be refining the database to follow specified business rules. This project is an extension of the database and will not support a fully functioning model.

## <b>Business Rules</b>

1. The people have accounts in the system with their ID, name, email , cellphone number. 
2. There are specific locations on campus where the food can be delivered
3. People can also be the delivery drivers and they have their license number, date they were hired and ratings.
4. Theres a fee of $5 for each delivery,  An individual delivery is tied to one and only one person, the order is for one resturant only. There will need to be a total price, delivery charge, and driver delivery time
5. The resturants have to be approved first before being added to the database, the information will require their location, ID, schedule, and a link to a website
6. Ratings will be based out of 5 stars and will give the user to ability to add a comment. The ratings will stay with the delivery user ID.
7. The database will have valuable nutrition information and eating habits


## <b>EERD Diagram</b>

![UpdatedERDDeliverable3](https://user-images.githubusercontent.com/78045412/114319999-db26bc00-9ae1-11eb-9195-a6cb32954c34.png)


## <b>Use Case</b>

![Rating System](https://user-images.githubusercontent.com/78045412/113455609-17b73100-93d9-11eb-9441-16d10cd8318e.png)


## <b>Data Dictionary</b>
![Screenshot (132)](https://user-images.githubusercontent.com/81653751/113455710-58af4580-93d9-11eb-983d-7f9f0066128c.png)
![Screenshot (133)](https://user-images.githubusercontent.com/81653751/113455711-59e07280-93d9-11eb-8396-d99d416c49e2.png)
![Screenshot (134)](https://user-images.githubusercontent.com/81653751/113455713-5baa3600-93d9-11eb-8e4c-821b22e85f2a.png)
![Screenshot (135)](https://user-images.githubusercontent.com/81653751/113455715-5cdb6300-93d9-11eb-95d5-c623b5cbbf53.png)
![Screenshot (136)](https://user-images.githubusercontent.com/81653751/113455716-5e0c9000-93d9-11eb-885c-bf88db227d32.png)
![Screenshot (137)](https://user-images.githubusercontent.com/81653751/113455722-61078080-93d9-11eb-8024-f0bf24f334a6.png)


## <b>Stored Procedure</b>
![StoredProcedure](https://user-images.githubusercontent.com/78045412/116761793-927a6880-a9e6-11eb-99f4-4b59cb0d49ed.png)


## <b>Advanced View</b>
<b>Query 1</b>

![Query1](https://user-images.githubusercontent.com/37620953/117174036-560a8c00-ad9b-11eb-83a7-c163d61df6f8.png)

<b>Query 2</b>

![Query2](https://user-images.githubusercontent.com/37620953/117173995-4e4ae780-ad9b-11eb-93e3-c3cb1b119221.png)




## <b>Report of Indexes</b>

Our project's database consists of 13 unique tables each eventually having a relationship to the main table which is the order table. Six of these tables connect directly to the orders table. Each entry of the six tables has their own unique foreign key to link to the order table. Through the course of the project, our team examined and implemented optimizations to the database. The idea of query optimization is to be able to execute a SQL command as efficiently as possible. It is essential to avoid unncessary commands or keywords. For example, the use of the wildcard tag '%' is considered unoptimal. It is best to specify as precisely as possible what entry the database manager is looking for. As you can see in the 2 advanced view queries, we have optimal SQL command usage. Each of the indexes that were queried did not require the use of wildcard tags, inner joins, or unnecessary union clauses.
