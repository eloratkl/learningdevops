#Task 1b: Automate the entire process of creating, updating, destroying the S3 bucket and cloudfront

#Steps taken -- Automation of handling S3 bucket (Approach adopted using Python boto3)
Pre-requisites involved
1. Install and configure the AWS SDK for Python (Boto3) https://docs.aws.amazon.com/cloud9/latest/user-guide/sample-python.html#sample-python-sdk
2. Have the access key id and secret access key ready https://docs.aws.amazon.com/powershell/latest/userguide/pstools-appendix-sign-up.html
3. To create a new configuration for AWS CLI 
   aws configure
   AWS Access Key ID [None]: accesskey
   AWS Secret Access Key [None]: secretkey
   Default region name [None]: region nearest to you
   Default output format [None]: json

