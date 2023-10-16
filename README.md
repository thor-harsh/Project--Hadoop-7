# Project--Hadoop-7

<table>
  
  **In this project we use the power of HBase and RESTful service to find the movie ratings for a given user id using python script.<br></br>**
  **Before diving into the dataset lets get to know what is HBase**?<br></br>

  Apache HBase is an open-source, NoSQL, distributed big data store. It enables random, strictly consistent, real-time access to petabytes of data. HBase is very effective for handling large, sparse datasets.<br>
HBase integrates seamlessly with Apache Hadoop and the Hadoop ecosystem and runs on top of the Hadoop Distributed File System (HDFS) or Amazon S3 using Amazon Elastic MapReduce (EMR) file system, or EMRFS. HBase serves as a direct input and output to the Apache MapReduce framework for Hadoop, and works with Apache Phoenix to enable SQL-like queries over HBase tables.<br></br>

  **This dataset which we downloaded contains 4 columns:** <br></br>
  **(UserId):** The user id of person who rated the movie<br></br>
  **(Movie-Id):** The movie id of movie which users rated<br></br>
  **(Ratings):** The ratings which the user gave to the given movie<br></br>
  **(Timestamp):** The time at which the user rated the given movie<br></br>

  **The different layers of our project is like this**:<br></br>
  
  1.**Top most layer is Python Client**-Here we wrote the code to connect to RESTful service which is itself connected to HBase which is in turn built on top of HDFS.<br></br>
  
  2.**Next layer is RESTful service**- which we connected to HBase which will help in getting pull and get request from outside the cluster to HBase which is inside the cluster to perform different set of operations as needed by the users.<br></br>

  3.**Next layer is HBase**- which read in data do the operation or perform the queries on that and then read it to the output to the user or serves it to the user through RESTful service.<br></br>

  4.**Final layer is HDFS**- which is the Hadoop Distibution File System which distibutes the work among different clusters of computers.<br></br>

  Application of this project can be in making a full fletched **Movie Recommendation System**.<br></br>

  **Important Note: Please go through the dataset once before going to the code.**


</table>


**So what are you waiting for...? Jump to the code to get started. As usual for any doubt or query see you in pull request section 😁😂. Thanks!**
