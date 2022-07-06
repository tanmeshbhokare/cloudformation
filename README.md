# CloudFormation
AWS CloudFormation is infrastructure as code (IaC) service that allows you to easily model, provision, and manage AWS and third-party resources. 

I've created this repository to store Sample CloudFormation templates

Task 1 : Create an AWS CloudFormation to create a bucket and lambda function.
  In the above yaml file, I've written a cloudformation template which creates a lambda funtion and integrates S3 bucket to it,
  so whenever file is uploaded to s3 bucket, it will trigger lambda function.
  that lambda function reads the contents of file, prints it and later delete from bucket.
  
  you can change the python function according to your requiremennt. 
