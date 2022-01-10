Covid-19 Data Engineering With AWS(cloud service)

 In this Project, I will get data from AWS dataset and make that data Cleaned, Perform some Transform and store that Structured data into Data-Warehouse...

--------------------------------------------------------------------------
Note: I'm going to use following AWS Services for getting job Done..
    
    1) AWS IAM
    2) AWS VPC
    3) AWS Athena
    4) AWS S3
    5) AWS Glue(crawler)
    6) AWS Redshift
    
    and Use Jupiter Notebook For Python code...
---------------------------------------------------------------------------

# Agenda Of Our Project...
============================================================
                            Phase-1 (Extract)
============================================================
 
 1) Find covid data for data analysis from aws dataset website : ("https://aws.amazon.com/covid-19-data-lake/")
 2) Upload that data in s3 bucket named "paras-de-covid-project".
 3) Create Database into AWS Athena.
 4) AWS athena for query the data which presented in CSV and JSON format.
 5) to load data into AWS athena we'll use AWS glue crawler 
 6) create crawler and set it up for crawl into s3 bucket.
 7) finally, we collected all data from s3 bucket to AWS athena successfully.
 
 
============================================================
                            Phase-2 (Transform)
============================================================                            
 
 1) create Relational datamodel for that data presented in "covid_19" database.
 2) Create Dimensional model for store data into data warehouse(AWS Redshift).
 3) Connect AWS Athena and Query the data.
 4) Write ETL job in Python.
 5) Transform data using python Pandas library done : (set Proper head of dataframe('static_datasetsstate_abv'),
                                                       Extracting date for 'dimDate' table which'll store into AWS Redshift)
 6) finally, we store that data from ETL into staging area (AWS S3).

 
 ===========================================================
                            Phase-3 (Load)
============================================================

 1) Create Cluster on AWS Redshift and connect with it using pyhon (redshift_connector) library.
 2) Build tables on AWS Redshift.
 3) copy data(Cleaned & Transformed) from AWS S3 to AWS Redshift.
 
 
 DONE!! 
