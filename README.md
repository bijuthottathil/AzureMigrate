# Setting up Azure Migrate Appliance for Seamless VM Migration to Azure

New Resource group created to keep Azure Migrate project


We have to start with Discover option

![image](https://github.com/user-attachments/assets/58ee0ce5-0ee5-4395-8536-c333692519c5)


Select Appliance ---> 3rd option Physical
![image](https://github.com/user-attachments/assets/a74389a6-8409-4e63-a0b0-5be96ab3fa56)



Create key- I put name awskey

Key will be downloaded in your machine. Please note down the key


![image](https://github.com/user-attachments/assets/c3e7a2d0-9d44-4143-aff7-bbefd8925a2e)


Now we need to create one EC2 instance in AWS. This EC2 machine  will be migrated to Azure in this tutorial

![image](https://github.com/user-attachments/assets/a65dddfd-8a4f-4f50-a10d-24cf92d96e74)
![image](https://github.com/user-attachments/assets/6ce45fea-1e49-4210-ab0f-4b2adc42a696)

Downloaded appliance software in AWS Windows Server

![image](https://github.com/user-attachments/assets/0f2382e3-bd34-4bb5-a082-37eb688d8851)


Open powershell sce and run the installer file

![image](https://github.com/user-attachments/assets/f069fc88-e96e-4c36-9b20-061827a3f4a4)


choose 3 rd option

![image](https://github.com/user-attachments/assets/181fcd01-ade1-4b0d-82fe-4ad94f48b891)


Selected scenario: Physical 
[OK]

1. Azure Public 
2. Azure US Government 
3. Azure China
Please enter the option for desired cloud [1, 2 or 3]: 1



Selected cloud: Azure Public 
[OK]

1. Set up an appliance for a Migrate project created with default (public endpoint) connectivity
2. Set up an appliance for a Migrate project created with private endpoint connectivity
Know more about the private endpoint connectivity: https://go.microsoft.com/fwlink/?linkid=2155739
Please enter the option for desired configuration [1 or 2]: 1

![image](https://github.com/user-attachments/assets/e6eb0c1d-395c-44e0-8a96-f7352c99b1a6)



![image](https://github.com/user-attachments/assets/4bca85e2-724e-4149-adf2-71c37066198b)


![image](https://github.com/user-attachments/assets/716bb10b-f39a-4435-a69c-c5822ceadbf2)

![image](https://github.com/user-attachments/assets/1e0e3de2-cb66-4fe3-86ad-ca9ed54b1a67)

After 30 mnts, installation completed
![image](https://github.com/user-attachments/assets/9180fc4b-68df-4cf7-a432-795961a868bc)

After installation of other script, it will open a browser with configuration check details

![image](https://github.com/user-attachments/assets/4e7a6dd2-9b23-44c6-9570-c753931aea6c)

![image](https://github.com/user-attachments/assets/91db57d8-2f9f-4cac-b86e-756121214628)

Next step is to login with Azure Credentials

It will popup a code and ask to login to azure account


![image](https://github.com/user-attachments/assets/77c10b6f-19fd-4dc6-b4a7-834dbff67016)

Moving to discovery part

![image](https://github.com/user-attachments/assets/b8a9ea32-5c19-4030-bc13-72b788562fec)

![image](https://github.com/user-attachments/assets/e9898954-d491-4a8c-9316-6c1410a0e4ed)


Next we need to choose our resource to migrate to Azure

![image](https://github.com/user-attachments/assets/d89a6529-b5d6-4b78-86c2-0846d497ba13)


I have created another AWS Windows VM to migrate to Azure
![image](https://github.com/user-attachments/assets/dfc49ec8-9874-4b89-9e83-addb5eb9f08c)



![image](https://github.com/user-attachments/assets/1b484478-1c09-4d5d-a8f0-7f9e7a029e91)

Below new EC2 Server I selected to migrate

![image](https://github.com/user-attachments/assets/17391f3b-413b-4262-a069-3e91ed3a8b38)

![image](https://github.com/user-attachments/assets/0e79f508-6f56-47df-a521-ecab063661c9)


Make sure that you VM got appropriate in bound rule for 5985, otherwise you will get error

![image](https://github.com/user-attachments/assets/0ac1b928-5da1-4567-bc8b-b8eb0018d00e)

![image](https://github.com/user-attachments/assets/0e4d9baa-685a-47d9-9c46-f3d1677779ba)

start discovery.. It can take some time

![image](https://github.com/user-attachments/assets/dfbd5433-902a-43b0-92d2-1bd5f7cd871c)


Discovery got completed

![image](https://github.com/user-attachments/assets/028975b3-3f33-4e97-9d42-1a7a11fc2ee0)

![image](https://github.com/user-attachments/assets/91c6d4c4-222d-4d26-883e-26bb43d56e5e)

![image](https://github.com/user-attachments/assets/af253bf4-4e07-4894-bd20-364420c4e716)

![image](https://github.com/user-attachments/assets/c1e3e75b-3f46-47e1-8fd8-bfdce8112b55)

Next step is to do assessment
![image](https://github.com/user-attachments/assets/8e87b7d2-63a5-4ac2-9918-d4e5a219fb4b)

![image](https://github.com/user-attachments/assets/e3db40b0-2fd0-4fe3-9cc8-4b07e74b857e)

![image](https://github.com/user-attachments/assets/6d4fad3f-94b9-45db-8194-0df702e663a5)

![image](https://github.com/user-attachments/assets/ccaa3f34-437d-45c5-a09f-35bc95653695)


![image](https://github.com/user-attachments/assets/0f573a50-d1dd-403d-b32e-9a8c6790a711)


Additional log analyst workspace to be installed

![image](https://github.com/user-attachments/assets/62aabe60-e3bf-4c09-87ea-ff606d596446)

![image](https://github.com/user-attachments/assets/83b8567b-9f66-47ba-a4b0-ef20b8822062)


![image](https://github.com/user-attachments/assets/c0df49e5-511a-4688-bddf-379df3802543)

![image](https://github.com/user-attachments/assets/4800555a-7974-4251-b5f7-7b02a543d624)

Assessment is completed


![image](https://github.com/user-attachments/assets/73870b4e-931e-435f-9751-e4d8d93aade9)


Now we will start migration process

![image](https://github.com/user-attachments/assets/2b9117aa-3aa4-44c7-8bf9-62aa069041e0)


We need to create new replicating VM in Azure

![image](https://github.com/user-attachments/assets/201c7695-ed00-483a-8b4c-b3557c1931e1)

![image](https://github.com/user-attachments/assets/939b383a-120d-4257-a022-aa194b80e105)

![image](https://github.com/user-attachments/assets/eec4f3ed-f096-4131-a3c9-6db72a9c2dd0)


Creating a replication server in AWS above windows 2016

Server created
![image](https://github.com/user-attachments/assets/a69f19ac-3087-4b7a-86d3-a85b046a55e1)




Install agent and disable all firewall options

installing agent


![image](https://github.com/user-attachments/assets/6d3c938d-e91b-4831-9e45-3cda4683e28d)

