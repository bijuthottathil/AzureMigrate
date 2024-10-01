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


