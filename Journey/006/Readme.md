## AWS Lambda with the AWS CLI 

## **Prerequisite**

Need to install the Windows subsystem for Linux to get a windows-Integrated version of Ubuntu and Bash

- Open powershell and run it as adminstrator and type this command: dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart 

<img width="642" alt="LinuxWin_1" src="https://user-images.githubusercontent.com/44376898/89755788-7e2bbf80-da95-11ea-903b-42a9cd0cd577.png"> 

- Install Linux distubution from Microsoft store

<img width="834" alt="LinuxWin_2" src="https://user-images.githubusercontent.com/44376898/89755987-13c74f00-da96-11ea-9ed0-22cff1b05d46.png"> 

- Restart your machine and do intial setup 

- Download and install aws cli on linux machine : curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" 

- unzip the package : unzip awscliv2.zip. Zipping might not work, install zip: *sudo apt install zip*
 
 - Run the install program: sudo ./aws/install 

### create the execution role 

- Create *Create-role command* , The trust-policy.json file is a JSON file in the current directory that defines the trust policy for the role. This trust policy allows Lambda to use the role's permissions by giving the service principal lambda.amazonaws.com permission to call the AWS Security Token Service AssumeRole action

- $ aws iam create-role --role-name lambda-ex --assume-role-policy-document '{"Version": "2012-10-17","Statement": [{ "Effect": "Allow", "Principal": {"Service": "lambda.amazonaws.com"}, "Action": "sts:AssumeRole"}]}' 
<img width="886" alt="LambdaCli_1" src="https://user-images.githubusercontent.com/44376898/89757528-630f7e80-da9a-11ea-916a-e19f7c7783cb.png">

- To add permissions to the role, use the attach-policy-to-role command 
<img width="830" alt="LambdaCli_2" src="https://user-images.githubusercontent.com/44376898/89757788-1e381780-da9b-11ea-85a5-00bfe510d740.png">

Will Create the function tomorrow 
