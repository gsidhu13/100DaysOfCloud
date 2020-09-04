## TOPIC - AWS Batch

I'll be honest, I had to research and understand what batching is. Batching is basically running a job or program in the background without user's interaction.

AWS Batch is a regional service, you could batch jobs acroos multiple availability Zones.

### Components

- **Jobs** : Collection of commands that you submit to AWS batch to run. Jobs can be reference by other jobs by name or by ID and can be dependent on the successfull completion of other jobs

- **Job Definations** : how you want to run your job. You specifiy roles, CPU and memory when you create a job.

- **Job Queues** : when you create a job, you submit to a particular queue, where it resides until it is scheduled onto a computer environment. 

- **Compute Environment** : A compute environment is a set of managed or unmanaged resources that are used to run jobs. 

### Running batch jobs at scale for less https://aws.amazon.com/getting-started/hands-on/run-batch-jobs-at-scale-with-ec2-spot/ 

**Prerequisites** 

If you never used EC2 spot instance, you need to create a few IAM roles: AmazonEC2SpotFleetRole, AWSServiceRoleForEC2Spot and AWSServiceRoleForEC2SpotFleet 

- Create *AmazonEC2SpotFleetRole* IAM role and attach *AmazonEC2SpotFleetTaggingRole* policy to *AmazonEC2SpotFleetRole*


    <img width="720" alt="20 1" src="https://user-images.githubusercontent.com/44376898/92207703-8251bf80-ee3e-11ea-8190-5c10e68302b3.png">

- Create *AWSServiceRoleForEC2Spot* and *AWSServiceRoleForEC2SpotFleet* service linked roles for EC2 Spot 

    <img width="819" alt="20 2" src="https://user-images.githubusercontent.com/44376898/92207712-867ddd00-ee3e-11ea-8369-083484cb067c.png">

Please refer to the link above for pictures reference, I am not creating my own content here so please refer to aws tutorial pictures

1. Go to Services, Select **Batch** under compute. Choose *Get started* and then choose **Skip wizard** under Define job.

2. 
