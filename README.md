# BigQuery_CloudSQL

SQL (Structured Query Language) is a standard language for Data Ops that allows DBA to query from structured datasets. 

It's commonly used in DB mgmt and allows to perform tasks like transaction record writing into relational databases and do DA (petabyte-scale data analysis).

This is a data science topics. This lab is divided into two parts: 

in the first half, you will learn how to export subsets of the London bikeshare dataset into CSV files, which you will then upload to Cloud SQL. From there you will learn how to use Cloud SQL to create and manage databases and tables. Towards the end, you will get hands-on practice with additional SQL keywords that manipulate and edit data.

In the second half, you will learn fundamental SQL querying keywords, which you will run in the BigQuery console on a public dataset that contains information on London bikeshares.

# Core Steps:

(1) Create Cloud SQL instance, config AC.

(2) uoload CSV data to Storage/Bucket

(3) util Google Big Data Production Tool called Big Query

--------------

from step 1:

> create Cloud SQL instance 

* 1.1, in cloud console, navigate to Storage >> Browser, click on "Create Bucket".


    ![storage bucket](https://cdn.qwiklabs.com/MJaLpJcY4bF7yM0I4XC%2BlzCe3F32kXqqayPLGZ5vK4Q%3D)
    
* 1.2, upload CSV data to the newly created Cloud Storage Bucket.

    ![upload](https://cdn.qwiklabs.com/O0gGDUAw3%2BKFgvwpeQvYtmRFgfAlChH09mZMXpztL%2FM%3D)

* 1.3, navigate to Storage >> SQL, then click on "create Cloud SQL instance".

    ![cloud sql instance](https://raw.githubusercontent.com/QueenieCplusplus/BigQuery_CloudSQL/main/sql_instance.png)

* 1.4, check the user & password to do Access Control to DB.

    ![AC](https://raw.githubusercontent.com/QueenieCplusplus/BigQuery_CloudSQL/main/AC.png)

* 1.5, Cloud SQL Instance is created then.

    ![](https://raw.githubusercontent.com/QueenieCplusplus/BigQuery_CloudSQL/main/cloud_sql_instance_created_1.png)

* 1.6, activate Cloud Shell.

![gcloud](https://raw.githubusercontent.com/QueenieCplusplus/BigQuery_CloudSQL/main/Cloud%20Shell.png)

* 1.7, type cmd line in shell.


