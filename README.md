# NYC-TAXI-ETL--project
This is an end-to-end Azure Data Engineering project using cutting-edge technologies like Azure Data Factory, Databricks, PySpark, and Delta Lake.

![image](https://github.com/user-attachments/assets/79ffc772-5973-4a2e-bfd7-fc8fd5038b10)

Data Source Link : https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page

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




































