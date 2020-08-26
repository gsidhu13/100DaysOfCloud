## TOPIC - Amazon EC2

Studing/Reading User Guide Linux instances https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/get-set-up-for-amazon-ec2.html 

**What is EC2?** Basically a virtual machine hosted in the cloud.

EC2 Instances are hosted on multiple locations worldwide:

**Regions**: AWS has multiple regions in multiple countries

**Availability Zone**: isolated Datacenter locations in each regions, AWS has multiple AZs within each region

**Local Zones** : have their own internet connections and support AWS Direct connect, Datacenter that are connected to AZs, could you close to end-users to provide low latency

**AWS Outposts**: fully managed service that extends AWS infrastructure, services, APIs, and tools to customer premises


### Create a key pair

Linux instances don't have password; you use a key pair to connect to Linux EC2 instances. Specify the key pair when you launch your instance, then provide the provide key when you log in using SSH 

1. Open EC2 Console, choose key pairs in Resources window or in the navigation pane under *Network and Security* and then choose *Create key pair*

<img width="1083" alt="Day12_1" src="https://user-images.githubusercontent.com/44376898/91258714-e0d1bc00-e721-11ea-9fb7-ac14f6d6dad0.png">
<img width="620" alt="Day12_2" src="https://user-images.githubusercontent.com/44376898/91258815-1bd3ef80-e722-11ea-9dad-25387357d7d0.png">

2. Name your key pair, select a file format and then choose *Create key pair*

<img width="499" alt="Day12_3" src="https://user-images.githubusercontent.com/44376898/91258960-681f2f80-e722-11ea-95d1-357af4d463e8.png">

