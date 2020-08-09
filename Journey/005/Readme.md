### **AWS CLI**

Managing AWS Services via CLI; AWS CLI provides direct access to all public APIs of AWS and you can build your own bash scripts to managed services

### **HOW TO CONNECT TO AWS CLI?**

   Linux- use bash

   Windows-Command Prompt

   Remotely- Run commands on EC2 using putty
   
 ### **Installing AWS CLI on Windows**
 
 Download MSI file and install it
 
 **Check AWS Version on Cmd** aws --version 
 
 ### **Uninstalling AWS CLI**
 
 - Remove it from program and feature 
 
 - From Cmd: appwiz.cpl
 
 ### **Configuring AWS CLI**
 
 You need to obtain Access Key ID, Secret Access Key, AWS Region, and output format
 
 **Create Access Key for an IAM user**
 
 - Sign in to management console, open IAM console and select users
 <img width="695" alt="AWSCLI_1" src="https://user-images.githubusercontent.com/44376898/89727369-f8e2d500-d9d8-11ea-9478-cc6f92b0e8d7.png">
 
 - select a user
 <img width="811" alt="AWSCLI_2" src="https://user-images.githubusercontent.com/44376898/89727404-5d059900-d9d9-11ea-99f1-dccd26f75c30.png">
 
 - Go to Security credentials and click on create acces key
 <img width="960" alt="AWSCLI_3" src="https://user-images.githubusercontent.com/44376898/89727522-938fe380-d9da-11ea-90ee-acadd5f9eede.png">
 
 - Grab your access Key ID and secret access key
 <img width="777" alt="AWSCLI_4" src="https://user-images.githubusercontent.com/44376898/89727533-b15d4880-d9da-11ea-8997-1b9179d72867.png">
 
- you could also download .csv file that contains access key ID and secret access key and store it for future use
 
 **Region**
 - it's usually the one close(us-west-2) to you but it can be any region
 
 ** Output Format** 
 
Needed to know and tell how you want to format your output, json is used by default 

**All the settings(credentials) are stored in profile. AWS uses default(file name) profile but it can be renamed (aws configure --profile produser).This command can also be used to update existing default profile**

**To only modify a single value i.e. region or output, use those as parameters( aws configure --region)

Finally configured the aws cli

<img width="570" alt="AWSCLI_5" src="https://user-images.githubusercontent.com/44376898/89727855-44977d80-d9dd-11ea-8f1e-c79a4a77412c.png">





 

 
 
 
 
 




