# Project--Hadoop-7

<table>
  
  **In this project we use the power of HBase and RESTful service to find the movie ratings for a given user id using python script.<br></br>**

  **This dataset which we downloaded contains 4 columns:** <br></br>
  **(UserId):** The user id of person who rated the movie<br></br>
  **(Movie-Id):** The movie id of movie which users rated<br></br>
  **(Ratings):** The ratings which the user gave to the given movie<br></br>
  **(Timestamp):** The time at which the user rated the given movie<br></br>

  **The different layers of our project is like this**:<br></br>
  
  1.Top most layer is Python Client-Here we wrote the code to connect to RESTful service which is itself connected to HBase which is in turn built on top of HDFS.<br></br>
  
  2.Next layer is RESTful service which we connected to HBase which will help in getting pull and get request from outside the cluster to HBase which is inside the cluster to 
  perform different set of operations as needed by the users.<br></br>

  3.Next layer is HBase which read in data do the operation or perform the queries on that and then read it to the output to the user or serves it to the user through RESTful service.<br></br>

  4.Final layer is HDFS which is the Hadoop Distibution File System which distibutes the work among different clusters of computers.<br></br>
