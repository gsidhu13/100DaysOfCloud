## TOPIC - AWS IAM - Users 

**Important points**

- Amazon resource name(ARN) of user is unique in across all of AWS.
- New users created in AWS cli don't have credentials/password by default. 
- A brand new user has no permissions at all.

### Managing Users

### View IAM user

**List all users in the account**

- *AWS Console* : In IAM navigation pane, choose users, it should display all the users

<img width="763" alt="Day11_1" src="https://user-images.githubusercontent.com/44376898/91132193-f8e20680-e661-11ea-981e-b2190a8fbeeb.png">

- *AWS CLI* : aws iam list-users

<img width="454" alt="Day11_2" src="https://user-images.githubusercontent.com/44376898/91133817-6d1caa00-e662-11ea-9c02-5b8101b8c985.png">

** To list users in a specific group
