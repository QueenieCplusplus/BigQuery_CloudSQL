# BigQuery_CloudSQL

SQL (Structured Query Language) is a standard language for Data Ops that allows DBA to query from structured datasets. 

It's commonly used in DB mgmt and allows to perform tasks like transaction record writing into relational databases and do DA (petabyte-scale data analysis).

This is a data science topics. This lab is divided into two parts: 

in the first half, you will learn how to export subsets of the London bikeshare dataset into CSV files, which you will then upload to Cloud SQL. From there you will learn how to use Cloud SQL to create and manage databases and tables. Towards the end, you will get hands-on practice with additional SQL keywords that manipulate and edit data.

In the second half, you will learn fundamental SQL querying keywords, which you will run in the BigQuery console on a public dataset that contains information on London bikeshares.

# Core Steps:

(1) uoload CSV data to Storage/Bucket.

(2) Create Cloud SQL instance, config AC.

(3) Create Connection between Storage/Bucket to SQL instance.

(4) util Google Big Data Production Tool called Big Query

--------------

# Storage Bucket

from step 1:

> upload Data to Storage Bucket

* 1.1, in cloud console, navigate to Storage >> Browser, click on "Create Bucket".


    ![storage bucket](https://cdn.qwiklabs.com/MJaLpJcY4bF7yM0I4XC%2BlzCe3F32kXqqayPLGZ5vK4Q%3D)
    
* 1.2, upload CSV data to the newly created Cloud Storage Bucket.

    ![upload](https://cdn.qwiklabs.com/O0gGDUAw3%2BKFgvwpeQvYtmRFgfAlChH09mZMXpztL%2FM%3D)
    
# Cloud SQL instance

from step 2:

> create Cloud SQL instance

* 2.1, navigate to Storage >> SQL, then click on "create Cloud SQL instance".

    ![cloud sql instance](https://raw.githubusercontent.com/QueenieCplusplus/BigQuery_CloudSQL/main/sql_instance.png)

* 2.2, check the user & password to do Access Control to DB.

    ![AC](https://raw.githubusercontent.com/QueenieCplusplus/BigQuery_CloudSQL/main/AC.png)

* 2.3, Cloud SQL Instance is created then.

    ![](https://raw.githubusercontent.com/QueenieCplusplus/BigQuery_CloudSQL/main/cloud_sql_instance_created_1.png)

# Connection using Cloud Shell

from step 3:

> activate Cloud Shell and type cmd line. (auth, project resource), then make it to connect with sql instance.

* 3.1, activate Cloud Shell.

![gcloud](https://raw.githubusercontent.com/QueenieCplusplus/BigQuery_CloudSQL/main/Cloud%20Shell.png)

* 3.2, type cmd line in shell, to check Project ID and auth Users Account.

         gcloud auth list
         
         [output]
         Credentialed accounts: -<username>@<hostname>.com (active)
     
         
         gcloud config list project
         
         [output]
         [Core]
         Project=<poj_id>
         
         [example output]
         Project=kates-gcp-1234567890abcedee
         // as above blue bar in step 1.5


* 3.3, make connection to sql.


