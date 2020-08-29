## TOPIC - AWS 

I am not reading a guide or documentation tonight, i am going to start doing random stuff on the portal and see where it leads me 

### How to Connect to EC2 from Windows system Linux 

1. Make sure WSL is connected to AWS console, use command - **aws configure** 
   
 - Get secret key and Access Key ID from the portal first 
  
      <img width="172" alt="15 1" src="https://user-images.githubusercontent.com/44376898/91630700-68b8ff80-e988-11ea-8b42-b5f767cb90b8.png">

      ## Issues

      - I am having trouble copying a key pair from windows to WSL. Not sure what's happening, I am following the instruction as documentation 

        <img width="425" alt="15 2" src="https://user-images.githubusercontent.com/44376898/91630750-dcf3a300-e988-11ea-8e0c-350cabbaf90e.png">

      - Turns out .ppk files are not compatiable with bash/WSL, it even says when you create a key pair. I"ll create new key pair this 

        <img width="359" alt="15 3" src="https://user-images.githubusercontent.com/44376898/91630840-d0237f00-e989-11ea-97b2-636da9bc44d5.png">

      - Can we assign new key pair to existing EC2? Not Really, you will need to create an AMI and launch new instance from that AMI. https://aws.amazon.com/premiumsupport/knowledge-center/ec2-windows-replace-lost-key-pair/

      - Finally got new key moved to WSL 


        <img width="259" alt="15 4" src="https://user-images.githubusercontent.com/44376898/91631693-55aa2d80-e990-11ea-987d-61a148e2667c.png">
    
2. You coud use SSH to connect to the instance, you need to have public DNS of your instance. Use this command: sudo ssh -i /path/my-key-pair.pem my-instance-user-name@my-instance-public-dns-name 

   - I was constantly getting this error, this post saved me : https://forums.aws.amazon.com/thread.jspa?threadID=143988 
   
      <img width="539" alt="15 5" src="https://user-images.githubusercontent.com/44376898/91632757-d15ba880-e997-11ea-86a3-03e2c0d9ac80.png">
      
    - Just noticed this instructions work like a charm 
    
    <img width="744" alt="15 6" src="https://user-images.githubusercontent.com/44376898/91632996-bab65100-e999-11ea-9faf-087ff28ddd9d.png">
    
    

   
