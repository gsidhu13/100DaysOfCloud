## TOPIC - IAM 

### How Users Sign In

1. Go to this link:https://signin.aws.amazon.com/console
    Users could manually enter in the account ID and then their credentials
    
2. Custom url:
    - Either create one https://*account-ID-or-alias*.signin.aws.amazon.com/console 
    - OR You could go to IAM dashboard, choose users, choose a user and then go to security credentials tab 
    - Copy the custom sign in URL
  <img width="908" alt="Day10" src="https://user-images.githubusercontent.com/44376898/90964177-10a76800-e473-11ea-8929-516b3fbdf25e.png">


### Tutorial on Billing Access

**Prerequisites**

1. Create two users
2. Create two groups and add users as a memeber 
<img width="1062" alt="Day10_1" src="https://user-images.githubusercontent.com/44376898/90965107-18b6d600-e47a-11ea-8c86-ed373d67d14f.png">

3. Make sure Access to billing is enabled. Refer to Day 09 

**Real work**

1. Create IAM policies that grant permissions to access billing information/data

- Sign in with adminstrator account, open IAM dashboard
- in the left/navigation pane, choose polices and then choose create policy

<img width="716" alt="Day10_2" src="https://user-images.githubusercontent.com/44376898/90965337-23726a80-e47c-11ea-81be-6152b597fedf.png">

- Select **Billing** services and then check box next to **All Actions**

<img width="817" alt="Day10_3" src="https://user-images.githubusercontent.com/44376898/90965383-8237e400-e47c-11ea-853d-73c40e8e1358.png">

- Review and create the policy

<img width="922" alt="Day10_4" src="https://user-images.githubusercontent.com/44376898/90965389-86640180-e47c-11ea-9c69-a1616ceb94d5.png">

- Create another policy and this check the box next top  **Read** instead of **All Actions**

<img width="891" alt="Day10_3" src="https://user-images.githubusercontent.com/44376898/90965515-a0eaaa80-e47d-11ea-8eba-71a729be2eff.png">


2. Attach policies to the groups 

- Go to IAM dashboard, in the navigation pane, choose groups
- Select the group, click on its permissions tab and then attach policy 
<img width="1020" alt="Day10_5" src="https://user-images.githubusercontent.com/44376898/90965595-63d2e800-e47e-11ea-91e1-6fa9076637cb.png">








