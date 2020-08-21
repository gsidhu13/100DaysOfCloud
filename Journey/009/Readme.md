## TOPIC - AWS IAM 

### Creating IAM Admin User and Group 

1. Sign in to the console using root account

2. Enable access to billing for this admin user that you will create
    - Click on **My Account** > **IAM User and Role Access to Billing Information** > Choose **Edit** > **Activate IAM Access** and update 
    <img width="674" alt="Day9_1" src="https://user-images.githubusercontent.com/44376898/90862826-de96e880-e342-11ea-8f0d-2fcd6664ed92.png">
    <img width="753" alt="Day9_2" src="https://user-images.githubusercontent.com/44376898/90863018-2cabec00-e343-11ea-8709-21011d26141c.png">
<img width="754" alt="Day9_3" src="https://user-images.githubusercontent.com/44376898/90863033-32093680-e343-11ea-98ca-c2b989242af7.png">

3. Go back to IAM dashboard, choose **Users** and then choose **Add User** 
    - Type username - **Administrator**
    - Select the check box for **AWS Management Console Access**, Select **Custom password**, type your password
    - Click **next:permissions** 
   
<img width="726" alt="Day9_4" src="https://user-images.githubusercontent.com/44376898/90864163-0d15c300-e345-11ea-82f0-df385ecdeab1.png">
<img width="1017" alt="Day9_5" src="https://user-images.githubusercontent.com/44376898/90864177-11da7700-e345-11ea-8595-bb6a9bb69a3f.png">
<img width="856" alt="Day9_6" src="https://user-images.githubusercontent.com/44376898/90864185-16069480-e345-11ea-907c-9841969a90e8.png">

4. Now create a group
    - Name the group - *Administrator*
    <img width="833" alt="Day9_7" src="https://user-images.githubusercontent.com/44376898/90864562-c07eb780-e345-11ea-86f5-9487875f6109.png">

