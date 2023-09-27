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





