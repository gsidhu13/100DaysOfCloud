## Topic - Amazon EC2 


### Launch an instance

1. Go to EC2 console and choose *Launch Instance*
    <img width="815" alt="14 1" src="https://user-images.githubusercontent.com/44376898/91393215-04166d00-e7ef-11ea-9ab5-2878c974038c.png">
    
2. Choose Free tier amazon Linux AMI 64 bit, we are selecting EBS-backed root device storage
    <img width="1041" alt="14 2" src="https://user-images.githubusercontent.com/44376898/91393269-08428a80-e7ef-11ea-9906-dc613f2985ef.png">
    
3. Choose an Instance type, select *t2.micro* instance type, it's eligible for free tier 
    <img width="899" alt="14 3" src="https://user-images.githubusercontent.com/44376898/91393317-0bd61180-e7ef-11ea-8cb9-84a411ee0053.png">

4. Keep the default options unless you want to add this instance to particular VPC/Subnet etc. You have others options avaiable too to avoid accidental termination. 
    <img width="926" alt="14 4" src="https://user-images.githubusercontent.com/44376898/91393355-0e386b80-e7ef-11ea-8486-437d3def1a9c.png">

5. Choose the default storage selected, skip tags and then choose security group. If choosing new security group, you will have option to add rules or you could select existing security group 
    <img width="1064" alt="14 5" src="https://user-images.githubusercontent.com/44376898/91393385-109ac580-e7ef-11ea-88b9-a45d4f2a8a54.png">
    <img width="1066" alt="14 6" src="https://user-images.githubusercontent.com/44376898/91393472-1690a680-e7ef-11ea-94cf-3844d864ce79.png">

6. On the Review Instance launch page, you could review your selections, choose launch and then choose an existing key pair
    <img width="497" alt="14 7" src="https://user-images.githubusercontent.com/44376898/91394559-82730f00-e7ef-11ea-8b11-21092cd8abe6.png">



