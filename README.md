# CloudFormation
AWS CloudFormation is infrastructure as code (IaC) service that allows you to easily model, provision, and manage AWS and third-party resources. 

I've created this repository to store Sample CloudFormation templates


Task 1 : Create an AWS CloudFormation to create a bucket and lambda function.

  In the above yaml file, I've written a cloudformation template which creates a lambda funtion and integrates S3 bucket to it,
  so whenever file is uploaded to s3 bucket, it will trigger lambda function.
  that lambda function reads the contents of file, prints it and later delete from bucket.
  
  you can change the python function according to your requirement. 


Task 2 : Create an AWS CloudFormation to create a bucket and trigger lambda function, also delete the objects from bucket while deleting CF Stack
  
  It is similar to Task 1, with delete capability
  
  Previously : if S3 Bucket is having any objects, CF stack will fail to delete S3 Bucket as it is not empty
  now whenever we delete CF Stack, lambda function will be triggered and it will delete objects from S3 Bucket and CF Stack will be deleted without any errors
  

Task 3 : Lambda function to create EC2 instance
  
  Create S3 Bucket and integrate lambda function to it, whenever file is uploaded to S3Bucket Lambda function will create an EC2 instance.
  Send S3Bucket to Outputs
  While Deleting CF Stack, it should delete EC2 Instance + S3Bucket (also delete objects from bucket) and all resources should be deleted.

Task 4 : display EC2 Instance id in outputs after lambda function is triggered 
  Lambda Function should create an EC2 instance and display instance-id in outputs tab
