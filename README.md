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
![Azure Instructions](https://imgur.com/aO7vezg)
4. If there is a successful connection, then click on the "ok" button. You should see it under "My SQL Connections" in your workbench. Double click to open up the connection. 
