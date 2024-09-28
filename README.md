# Setting up Azure Migrate Appliance for Seamless VM Migration to Azure

New Resource group created to keep Azure Migrate project
![image](https://github.com/user-attachments/assets/60054dcd-436f-4ca3-8515-b2138a231d07)


![image](https://github.com/user-attachments/assets/70ec0f3d-5b31-426e-ab2a-ccc15f0c51ba)


![image](https://github.com/user-attachments/assets/92af72d6-a06d-4b22-8c6a-e26a6a3f0b5c)

We have to start with Discover option

Select Appliance ---> 3rd option Physical


![image](https://github.com/user-attachments/assets/0fce7c24-f285-42de-92c4-8b8b6df7e13c)

Create key- I put name awskey

Key will be downloaded in your machine. Please note down the key


awskey;PROD;50c70d3e-8356-4111-82d3-3fb1deae449b;e3fe7a24-7f96-4d9e-bb03-a60836b78bbb;RG-Migrate;awstoazure;3c3a9488-c919-45f9-b060-db98bd2e4d05;df0a20f6-f09b-417a-a8f8-fa92776235d9;https://discoverysrv.wus2.prod.migration.windowsazure.com/;westus2;false

Now we need to create one EC2 instance in AWS. This EC2 machine  will be migrated to Azure in this tutorial
