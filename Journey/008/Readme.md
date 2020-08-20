
## TOPIC - IAM (Indentiy Access Management)

IAM allows us to manage access to AWS resources. IAM makes sure user must be able to authenticate(username and password) himself and have been authorized(permissions) to access AWS resources.

### IAM Feature

- **Free to use** - AWS IAM and AWS service token are free to use.
- **Granular permission** permissions to resources could be assigned at granular level. For instance, some users could have access S1 bucket in S3 while other users may not. 
- **Compatiability** - IAM works with almost all AWS resources, access to those resources can be managed using IAM
- **Login Logs** - if we use CloudTrail, we could also see what resources a particular user tried to access
- **PCI DSS complaince** - IAM supports the processing, storage, and transmission of credit card data by a merchant or service provider, and has been validated as being compliant with Payment Card Industry (PCI) Data Security Standard (DSS)
- **Idendity Federation** - IAM allows you access to access AWS resources using your credentials from another source i.e. facebook, gmail. It only provides temporary access to your account.

### How to Access IAM

- AWS Console
- AWS command line
- AWS SDKs
- AWS HTTPS API 

