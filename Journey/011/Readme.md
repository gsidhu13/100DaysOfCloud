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

    -  **Review Policy**

