# TOPIC - IAM

## Create and Attach Customer Mangaged Policy to an IAM user

We will create our own policy and attach it to a user, we won't attach the policy to a group like we have done in the past.

### Prequisites 

Create an IAM User, no group or permissions 

<img width="852" alt="Day10_8" src="https://user-images.githubusercontent.com/44376898/90972222-0a91a580-e4cc-11ea-9c04-f6538f50caad.png">

no permssions at all

<img width="712" alt="Day10_9" src="https://user-images.githubusercontent.com/44376898/90972225-0e252c80-e4cc-11ea-8606-72286b4914c6.png">


### Real work

1. **Create the Policy** 
    - Sign in to console and go to IAM dashboard
    - in the navigation pane, select Policies, choose **Create Policy**
    - In **JSON** tab, copy and paste the following text 
    
      {
    "Version": "2012-10-17",
    "Statement": [ {
        "Effect": "Allow",
        "Action": [
            "iam:GenerateCredentialReport",
            "iam:Get*",
            "iam:List*"
        ],
        "Resource": "*"
    } ]
}

    -  **Review Policy** , type *IAMConsoleReadOnlyAccess* for the policy name and then choose **Create policy** 
    
   <img width="593" alt="Day10_10" src="https://user-images.githubusercontent.com/44376898/90972412-a243c380-e4cd-11ea-8f87-436f3dabf048.png">
    <img width="898" alt="Day10_11" src="https://user-images.githubusercontent.com/44376898/90972413-a374f080-e4cd-11ea-90bc-624228515163.png">
    <img width="814" alt="Day10_12" src="https://user-images.githubusercontent.com/44376898/90972415-a4a61d80-e4cd-11ea-8fc5-326466e1fb77.png">
    
2. Attach Policy to the users

    - In the IAM console, choose Polcies in the navigation pane
    - Search for *IAMConsoleReadOnlyAccess* policy, choose **Policy Usage** tab and then choose **Attach**
    - Choose Users and then Select *CustomPolicyUser*
        
    <img width="1007" alt="Day10_13" src="https://user-images.githubusercontent.com/44376898/90972508-76750d80-e4ce-11ea-9386-d854b3522630.png">
    <img width="893" alt="Day10_14" src="https://user-images.githubusercontent.com/44376898/90972510-77a63a80-e4ce-11ea-96e0-decdb1d900a7.png">
    
    
3. Test user acccess

    Looks much different now
    
    
<img width="691" alt="Day10_15" src="https://user-images.githubusercontent.com/44376898/90972545-d8ce0e00-e4ce-11ea-8afd-b478a0765ca9.png">


    
    

