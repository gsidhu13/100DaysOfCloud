## TOPIC - AWS IAM - Users 

**Important points**

- Amazon resource name(ARN) of user is unique in across all of AWS.
- New users created in AWS cli don't have credentials/password by default. 
- A brand new user has no permissions at all.

### Managing Users

### View IAM users

**List all users in the account**

- *AWS Console* : In IAM navigation pane, choose users, it should display all the users

<img width="763" alt="Day11_1" src="https://user-images.githubusercontent.com/44376898/91132193-f8e20680-e661-11ea-981e-b2190a8fbeeb.png">

- *AWS CLI* : aws iam list-users

<img width="454" alt="Day11_2" src="https://user-images.githubusercontent.com/44376898/91133817-6d1caa00-e662-11ea-9c02-5b8101b8c985.png">

** To list users in a specific group**

- *AWS Console* : In the navigation pane, choose groups, choose a group, then choose the users

<img width="704" alt="Day11_3" src="https://user-images.githubusercontent.com/44376898/91138828-05675e80-e664-11ea-83e2-3c27d7b54eb4.png">

- *AWS CLI* : aws iam get-group --group-name **Adminstartors**

<img width="369" alt="Day11_4" src="https://user-images.githubusercontent.com/44376898/91138895-0a2c1280-e664-11ea-851c-28797ebd9e70.png">


**List all the groups that a user is in**

- *AWS Console*: In the navigation pane, choose users, choose user name and then choose the groups tab

<img width="669" alt="Day11_5" src="https://user-images.githubusercontent.com/44376898/91139837-4fe8db00-e664-11ea-9630-dbf845c582a7.png">

<img width="704" alt="Day11_3" src="https://user-images.githubusercontent.com/44376898/91139927-55debc00-e664-11ea-87f4-d47e77cd2942.png">

- *AWS CLI* : aws iam list-groups-for-user 

<img width="331" alt="Day11_6" src="https://user-images.githubusercontent.com/44376898/91140974-a2c29280-e664-11ea-8db7-708c8cc184c6.png">
