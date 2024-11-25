# NYC-TAXI-ETL--project
This is an end-to-end Azure Data Engineering project using cutting-edge technologies like Azure Data Factory, Databricks, PySpark, and Delta Lake.

![image](https://github.com/user-attachments/assets/79ffc772-5973-4a2e-bfd7-fc8fd5038b10)

Data Source Link : https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page

Reference project:https://www.youtube.com/watch?v=LQY2fvEv4cM&t=6035s&ab_channel=AnshLamba

Connect to ADLS Gen2 using python: https://learn.microsoft.com/en-us/azure/databricks/connect/storage/tutorial-azure-storage

1.create a resource group,storage account (with container names as Bronze,silver,gold),Data factory,key-vault,App registrations,Databricks

2.select the required file from the website-Right click on the file and copy the link address.

3.Create a linked service for source using HTTP

![image](https://github.com/user-attachments/assets/01fb1814-ecfc-4ce9-9f51-e5be4f5b16e4)

4.Create a linked service for sink using ADLS 

5.create source Dataset using HTTP,Parquet

![image](https://github.com/user-attachments/assets/2cc805f0-fb55-4b2b-b5bd-abd651250f19)

6.create sink dataset using ADLS,Parquet,select bronze container for file path

![image](https://github.com/user-attachments/assets/dcdcc630-264b-4279-8c8c-6f49f2f4680d)

7.Parametrize the source for getting all months data.

![image](https://github.com/user-attachments/assets/a733cd3c-6c73-4a92-9cce-c894e381f986)

8.add dynamic content

![image](https://github.com/user-attachments/assets/710a92ea-c677-40f5-a825-f1fbb937c6cc)

9.Do a for each activity

![image](https://github.com/user-attachments/assets/c3337363-2588-46df-8b74-ce89aa9340a5)

![image](https://github.com/user-attachments/assets/26d84c65-7fa2-4003-9765-76dbea0b009b)

10.in the copy activity-source-value-click on foreach activity

![image](https://github.com/user-attachments/assets/a4a680fe-ccd9-426a-9f32-b256ba51f6cd)

11.if the month is single digit it is working fine,but if it sis 2 digit its not working ,so kept an if-condition

![image](https://github.com/user-attachments/assets/7293a2bf-55ce-4c6f-bfe8-f1e31274910b)

12.hj

![image](https://github.com/user-attachments/assets/60eb3168-9bc9-4863-a971-77831298aed3)

13. in the true activity ,similar to what we have done previously like create a linked service,dataset,parameter

![image](https://github.com/user-attachments/assets/6de3985e-0d81-457b-8a3c-10e2e1e51640)

14.in the if condition-true

![image](https://github.com/user-attachments/assets/ce689e2a-6730-4499-943f-4464c1893f79)

15.create app registrations and copy  client id,scoped etc to connect to databricks.

![image](https://github.com/user-attachments/assets/dbcc074e-1e90-4569-b156-ae017f1773f7)

16.Import libraries

![image](https://github.com/user-attachments/assets/8054db7a-abf3-4e74-88b3-ccb884ca23e8)

17.Read csv file and display the data

![image](https://github.com/user-attachments/assets/74702d70-cdf3-4220-b592-8237131aeac6)



























