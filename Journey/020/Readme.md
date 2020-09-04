## TOPIC - AWS Batch

I'll be honest, I had to research and understand what batching is. Batching is basically running a job or program in the background without user's interaction.

AWS Batch is a regional service, you could batch jobs acroos multiple availability Zones.

### Components

- **Jobs** : Collection of commands that you submit to AWS batch to run. Jobs can be reference by other jobs by name or by ID and can be dependent on the successfull completion of other jobs

- **Job Definations** : how you want to run your job. You specifiy roles, CPU and memory when you create a job.

- **Job Queues** : when you create a job, you submit to a particular queue, where it resides until it is scheduled onto a computer environment. 

- **Compute Environment** : A compute environment is a set of managed or unmanaged resources that are used to run jobs. 


