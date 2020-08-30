## TOPIC - AWS Lambda

### Creating a Lambda function with AWS CLI

I think I should have done this on day 7 or day 8 but it never happpened, I picked a different topic next day. I'll be creating this function in WSL. I'll be following this guide: https://docs.aws.amazon.com/lambda/latest/dg/gettingstarted-awscli.html 

An escape character(\) is used to split a command over multple lines. 

1. First thing first, we need to create an execution role that will allow us to access AWS resouces i.e lambda.
    - we need to create *trust-policy.json* file and move to WSL directory and then runt this command: aws iam create-role --role-name lambda-ex --assume-role-policy-document file://trust-policy.json
2. Need to assign permissions to this role, we will use *AWSLambdaBasicExecutionRole* managed policy 

    <img width="526" alt="18 1" src="https://user-images.githubusercontent.com/44376898/91671651-746a0a80-eadd-11ea-9ce0-c6ef6abd4320.png">
    
3. Create index.js file with sample code and move the file to WSL directory 
    - Sample code: exports.handler = async function(event, context) {
  console.log("ENVIRONMENT VARIABLES\n" + JSON.stringify(process.env, null, 2))
  console.log("EVENT\n" + JSON.stringify(event, null, 2))
  return context.logStreamName
}

4. Deployment package file(index.js) must be zipped 

5. Now use *Create-function* command to create a lambda function 
    - *aws lambda create-function --function-name my-function \
    --zip-file fileb://function.zip --handler index.handler --runtime nodejs12.x \
--role arn:aws:iam::123456789012:role/lambda-ex*

      <img width="779" alt="18 2" src="https://user-images.githubusercontent.com/44376898/91671906-6cab6580-eadf-11ea-9f7a-b2bfb4039f1a.png">

6. Get logs for an invocation from the command line, use the --log-type option 
    - *aws lambda invoke --function-name my-function out --log-type Tail*
    
    <img width="581" alt="18" src="https://user-images.githubusercontent.com/44376898/91672011-5baf2400-eae0-11ea-9432-f8a42af12f54.png">

    
 7. How to view all of your functions? aws lambda list-functions --max-items 10. *max-items* allows you to view numbers of functions to view if you have 100s of functions.
 
    <img width="393" alt="18 4" src="https://user-images.githubusercontent.com/44376898/91672020-6bc70380-eae0-11ea-9dbe-f022f0b8424a.png">

 8. Clean up and delete your function
    -  aws lambda delete-function --function-name my-function
    
    <img width="369" alt="18 5" src="https://user-images.githubusercontent.com/44376898/91672030-75e90200-eae0-11ea-93a5-6537d8eac400.png">

    
    
