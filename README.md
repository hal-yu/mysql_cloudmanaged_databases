# mysql_cloudmanaged_databases
This assignment focuses on MySQL, and exploring its implementation on leading cloud platforms: Azure and GCP. By the end, you'll gain hands-on experience in setting up MySQL on these platforms, using MySQL Workbench to design, manage, and interact with your databases, and optionally connecting to your database using Python to retrieve data.

# Set Up Process from GCP

1. After clicking "Create an Instance," Click on Choose MySQL:
2. Create an Instance ID and password
3. Choose Cloud SQL edition as Enterprise and the preset edition as Sandbox
4. For Machine Configuration, change the dedicated core to shared core and choose the first option:
6.  Under connections, add a new network and enter 0.0.0.0/0 for the network and create instance on the bottom
## MySQL Workbench 
1. Open up MySQL Workbench and click on the "+" button
2. Insert a connection name
3. Copy and paste the IP address from GCP into the hostname
4. Click "Store in Vault" and enter your password you created the instance with.
5. Click on test connection and hopefully receieve a notification for a successful notification. 
6. If there is a successful connection, then click on the "ok" button. You should see it under "My SQL Connections" in your workbench. Double click to open up the connection. 

# Set Up Process from Azure
1. Under Azure Database for MySQL flexible servers, click "create" and select flexible server.
2. Create a server name, admin username, password, and confirm your password.
3. Click on the network tab on the top next to basics and select "Allow public access to this resource through the internet using a public IP address." Then on the bottom, select the "+ Add 0.0.0.0 - 255.255.255.255" and select continue. Then review and create your instance.
## MySQL Workbench 
1. Open up MySQL Workbench and click on the "+" button
2. Insert a connection name
3. Follow the steps under Azure to establish a connection.
[Azure Instructions](https://imgur.com/a/FuJrmFQ)
4. If there is a successful connection, then click on the "ok" button. You should see it under "My SQL Connections" in your workbench. Double click to open up the connection. 

# Creating ERD
- For the ERD, it was necessary to create new tables. These tables followed the format of the ones from the sample.
- First, a new database was created under the name "w4_assignments."
  ```Create database w4_assignments;```
- I have to move into the correct database
```use w4_assignments;```
- The table names "doctors" and "patients" were created using ![Professor Hants' code](https://github.com/hantswilliams/HHA_504_2023/blob/main/WK4/code/1_n_create.sql), but were slightly modified. Two other tables named "visits" and "appointments were created following the same format as the codes from doctors and patients. These tables include the column names (patient_id), data types (INT, VARCHAR(30)), and constraints (NOT NULL). The foreign key constraints for the table "doctor" was also established. The script can be found [Azure](https://github.com/hal-yu/mysql_cloudmanaged_databases/blob/main/Azure/ERD.sql) and [GCP](https://github.com/hal-yu/mysql_cloudmanaged_databases/blob/main/GCP/ERD.sql).
