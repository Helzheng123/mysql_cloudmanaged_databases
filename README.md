# mysql_cloudmanaged_databases
This assignment focuses on MySQL, and exploring its implementation on leading cloud platforms: Azure and GCP. By the end, you'll gain hands-on experience in setting up MySQL on these platforms, using MySQL Workbench to design, manage, and interact with your databases, and optionally connecting to your database using Python to retrieve data.

## Steps taken to set up MySQL on Azure and GCP:
#### GCP:
 - Log in with your Stony Brook email address
 - Go to <img width="79" alt="image" src="https://github.com/Helzheng123/mysql_cloudmanaged_databases/assets/123939070/4c05c685-9ed2-4bf7-be4b-ed481fcc16d5"> this drop-down and click on **NEW PROJECT**
 - Name the Project name **HHA504-WK4A-HW**. Keep the Organization as stonybrook.edu. Set the location to **AHI-GCP**
 - In the Project, click on the **Navigation Menu/Hamburger** <img width="16" alt="image" src="https://github.com/Helzheng123/mysql_cloudmanaged_databases/assets/123939070/f6224bc4-a62a-4936-9981-f6083ecff0fd"> and click on **SQL**
 - Click on **CREATE INSTANCE** and click on **MySQL**. Click on **ENABLE API**
 - Once the page brings you to a **Create a MySQL instance**,
    -  Set your Instance ID with your assignment name: I put mine as **helen-wk4a-assignment**. Then set your password.
    -  Keep the Database version as MySQL 8.0
    -  <img width="266" alt="image" src="https://github.com/Helzheng123/mysql_cloudmanaged_databases/assets/123939070/d6d4d3e0-3a18-4801-9879-fd109a018f97"> Choose **Enterprise** instead of Enterprise Plus
    -  <img width="266" alt="image" src="https://github.com/Helzheng123/mysql_cloudmanaged_databases/assets/123939070/11b0a323-1906-4226-bd41-970d4177f207"> Choose **Sandbox**
    -  <img width="174" alt="image" src="https://github.com/Helzheng123/mysql_cloudmanaged_databases/assets/123939070/d91a2ddd-36dc-41f1-ac0b-362164de78b3"> At **Customize your instance**, go to **Machine configuration** and choose **Shared core; 1 vCPU, 0.614 GB**
    -  At **Connections**, choose **Public IP** and **Add a network**; Name the network as **Allow All** and set it to **0.0.0.0/0**. Then press **Create Instance**
  
#### Azure:
 - Log in to Azure with Stony Brook email. Type in the search bar **Azure Databases for MySQL**. Once you click on it, click on **Create**.
 - Select **Flexible server**
 - Make sure the subscription is **Azure for Students**. Then create a new resource group: I named mine **helen-wk4a-assignment**
 - Create a server name: **hha504-wk4a-assignment**. Make sure the **Compute + Storage** section shows this: <img width="200" alt="image" src="https://github.com/Helzheng123/mysql_cloudmanaged_databases/assets/123939070/2c9681bd-5877-4a28-972d-98d15b3e8c0c">
 - Create an **Admin username** and set a password. Click **Next: Networking >**
 - Make sure the connectivity method is at **Public access (allowed IP addresses) and Private endpoint**.
 - Under **Firewall rules**, click on **Allow public access from any Azure service within Azure to this server**. Click on **+Add 0.0.0.0 - 255.255.255.255** <img width="150" alt="image" src="https://github.com/Helzheng123/mysql_cloudmanaged_databases/assets/123939070/e6d01285-8798-4ce0-9c78-c578c32fc698">
  - Then press **Create**

## MySQL Workbench for Database Interaction:
For GCP, it was relatively easy since we had gone over the process of connecting our instance with the MySQL Workbench. 

For Azure, it was a little more work to create the server, however, I followed this [guide](https://learn.microsoft.com/en-us/azure/mysql/flexible-server/connect-workbench) to figure out how to connect my server with MySQL Workbench. The only difference between Azure and GCP when creating the connection was the **Hostname** and **Username** options. For the **Hostname**, I copied and pasted my **Server Name** (example: **mydemoserver.mysql.database.azure.com**). For the **Username**, I put in the **server admin username** that I created when I was creating the **Azure Database for MySQL**. 

After connecting each service to MySQL Workbench, I successfully created an Entity Relationship Diagram in both the [GCP connection](https://github.com/Helzheng123/mysql_cloudmanaged_databases/blob/main/GCP/Screenshot%20of%20ERD%20diagram%20(GCP).png) and [AZURE connection](https://github.com/Helzheng123/mysql_cloudmanaged_databases/blob/main/AZURE/Screenshot%20ERD%20diagram%20(Azure).png). I used the same SQL scripts for both services and the [**patients**](https://github.com/hantswilliams/HHA_504_2023/blob/main/WK4/code/1_n_create.sql), [**doctors**](https://github.com/hantswilliams/HHA_504_2023/blob/main/WK4/code/1_n_create.sql), and [**demographics**](https://github.com/hantswilliams/HHA_504_2023/blob/main/WK4/code/1_1_create.sql) tables were taken from Professor Hants's Github. The other two tables: **appointments** and **laboratorytests** were created and added on my own.

Screenshots of each SQL command executed and their outcomes are shown in the [GCP](https://github.com/Helzheng123/mysql_cloudmanaged_databases/tree/main/GCP) folder (it was the exact same for Azure so I didn't upload the screenshots). 

Screenshots of a successfully run command are shown in each folder for each connection. 
