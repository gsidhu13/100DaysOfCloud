## TOPIC - EC2 Dashboard

I am aiming to open random stuff and learn about it. Going to learn importance of each thing 


**EVENTS**

  - AWS schedule instances termination, reboot, stop, maintenance and retirement. All thos scheduled events will be listed here.
  
**Instances**
  
  - All the instances are listed here, if an instance has been terminated recently, it will be listed for a little and then it will disappear. All running, stopped, hibernated will always be here
  
  - Settings icon at top right corner lets you modify instance's attribute
  
  <img width="535" alt="15 8" src="https://user-images.githubusercontent.com/44376898/91633902-facd0200-e9a0-11ea-8962-65351913ca3d.png">
 
**Lightsail**

  - It is lighter version of EC2 dashboard, things are very simplistic here, instances would have fixed amount of RAM and CPU
  - Cost effective, great for someone who wants to start migrating to AWS but don't want to learn all complex features
  - Security groups are keep it simple here.
  - Load balancer is available
  - This post on stackoverflow does a good comparison between EC2 and lightsail https://stackoverflow.com/questions/40927189/what-is-difference-between-lightsail-and-ec2
  - Short youtube video by AWS :https://www.youtube.com/watch?v=taMlabDBO58 
  
**Launch Template**

  - It allows you to save instance's configuration such as security group configs, network settings, key pair etc and launch it later
  - Launch template doesn't necessarily get used with ASG but launch templates are required when setting up auto scaling group 
  
  ### Creating a Launch Template
  
  - Go to EC2 dashboard, choose *launch templates* in the navigation pane, then choose *Create launch template*  
  
      <img width="750" alt="17 1" src="https://user-images.githubusercontent.com/44376898/91647650-f7be2a00-ea11-11ea-8bf2-8e36b2b70430.png">
  
  - Name your template, write description. *Source Template* allows you to create template from another template
  
     <img width="750" alt="17 2" src="https://user-images.githubusercontent.com/44376898/91647654-fdb40b00-ea11-11ea-9daf-1c56944fe0da.png">
     
   - Now Select *AMI*, if you are creating a template for ASG, it is required otherwise you could leave it the way it is. You may not be able to select your AMI from dropdown option, go to your AMI, copy the name and type it here.
   
      <img width="353" alt="17 3" src="https://user-images.githubusercontent.com/44376898/91647845-80d66080-ea14-11ea-8d92-2675187f0cd5.png">
      
   - Select *Instance type*, *Key Pair* and *Security Group*     
   - here you have option to add storage, tags and Network interface to the instance that will be launced. Advanced details allow you manages your instance's behavior such Capacity reservation, T2/T3 unlimited, RAM disk ID etc. It also include userdata. We will learn about those in next few days.
   - After reviewing your options, choose *Create launch template* 
   
      <img width="322" alt="17 4" src="https://user-images.githubusercontent.com/44376898/91647846-86cc4180-ea14-11ea-86de-9e9e7d91364e.png">
      
      <img width="323" alt="17 5" src="https://user-images.githubusercontent.com/44376898/91647847-8af85f00-ea14-11ea-9fba-e282b2481d56.png">
   
   
  
  
  
