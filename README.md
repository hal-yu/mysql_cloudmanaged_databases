# mysql_cloudmanaged_databases
This assignment focuses on MySQL, and exploring its implementation on leading cloud platforms: Azure and GCP. By the end, you'll gain hands-on experience in setting up MySQL on these platforms, using MySQL Workbench to design, manage, and interact with your databases, and optionally connecting to your database using Python to retrieve data.

# Set Up Process from GCP

1. After clicking "Create an Instance," Click on Choose MySQL:
```![image](https://github.com/hal-yu/mysql_cloudmanaged_databases/assets/124009232/351e3584-f99b-4664-9872-cf60b6b98358)```

2. Create an Instance ID and password
```![image](https://github.com/hal-yu/mysql_cloudmanaged_databases/assets/124009232/1a2eb887-8293-44e1-afd2-1dee432d0046)```

3. Choose Cloud SQL edition as Enterprise and the preset edition as Sandbox
```![image](https://github.com/hal-yu/mysql_cloudmanaged_databases/assets/124009232/e58282c1-e784-4918-94d8-d52b14d8ee7d)```

4. For Machine Configuration, change the dedicated core to shared core and choose the first option:
```![image](https://github.com/hal-yu/mysql_cloudmanaged_databases/assets/124009232/5f226a93-325c-4910-9a99-72d779837732)```

6.  Under connections, add a new network and enter 0.0.0.0/0 for the network and create instance on the bottom
```
![image](https://github.com/hal-yu/mysql_cloudmanaged_databases/assets/124009232/0c18420c-9a9b-49b5-8422-89c0df6b1c95)
![image](https://github.com/hal-yu/mysql_cloudmanaged_databases/assets/124009232/5ec48e36-2f5f-49fc-abdd-ab595a50611d)
```

## MySQL Workbench 
1. Open up MySQL Workbench and click on the "+" button
```![image](https://github.com/hal-yu/mysql_cloudmanaged_databases/assets/124009232/555f0839-a613-4295-b50d-25853b7909c4)```
2. Insert a connection name
3. Copy and paste the IP address from GCP into the hostname
```![image](https://github.com/hal-yu/mysql_cloudmanaged_databases/assets/124009232/282873a0-c648-4732-ad18-324f846298e2)```
```![image](https://github.com/hal-yu/mysql_cloudmanaged_databases/assets/124009232/80d9a2da-e37f-4b0d-aab2-22d45f377df7)```
4. Click "Store in Vault" and enter your password you created the instance with.
5. Click on test connection and hopefully receieve a notification for a successful notification. 
```![image](https://github.com/hal-yu/mysql_cloudmanaged_databases/assets/124009232/8b15a53b-0353-4744-9852-ba1ae3ba0f4d)```
6. If there is a successful connection, then click on the "ok" button. You should see it under "My SQL Connections" in your workbench. Double click to open up the connection. 

# Set Up Process from Azure
1. Under Azure Database for MySQL flexible servers, click "create" and select flexible server.
2. Create a server name, admin username, password, and confirm your password.
3. Click on the network tab on the top next to basics and select "Allow public access to this resource through the internet using a public IP address." Then on the bottom, select the "+ Add 0.0.0.0 - 255.255.255.255" and select continue. Then review and create your instance.
```
![image](https://github.com/hal-yu/mysql_cloudmanaged_databases/assets/124009232/c1df19b4-b600-4839-866f-c143d310fa79)
![image](https://github.com/hal-yu/mysql_cloudmanaged_databases/assets/124009232/341b264c-328d-4848-b3eb-facc632670eb)
```

## MySQL Workbench 
1. Open up MySQL Workbench and click on the "+" button
```![image](https://github.com/hal-yu/mysql_cloudmanaged_databases/assets/124009232/555f0839-a613-4295-b50d-25853b7909c4)```
2. Insert a connection name
3. Follow the steps under Azure to establish a connection.
```![image](https://github.com/hal-yu/mysql_cloudmanaged_databases/assets/124009232/e3f20546-02da-48d9-8052-fc8d2b8cbb10)```
4. If there is a successful connection, then click on the "ok" button. You should see it under "My SQL Connections" in your workbench. Double click to open up the connection. 
