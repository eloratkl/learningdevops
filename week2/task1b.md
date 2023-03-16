# Task 1b: Automate the entire process of creating, updating, destroying the S3 bucket and cloudfront
https://www.youtube.com/watch?v=QSvw50mMQaQ


# Automation of handling S3 bucket (Approach adopted using Python boto3)
Pre-requisites involved
1. Install and configure the AWS SDK for Python (Boto3) \
https://docs.aws.amazon.com/cloud9/latest/user-guide/sample-python.html#sample-python-sdk
2. Have the access key id and secret access key ready \
https://docs.aws.amazon.com/powershell/latest/userguide/pstools-appendix-sign-up.html
3. To create a new configuration for AWS CLI \
   aws configure\
   AWS Access Key ID [None]: accesskey\
   AWS Secret Access Key [None]: secretkey\
   Default region name [None]: region nearest to you\
   Default output format [None]: json
   
# Steps taken
1. List and create a S3 bucket \
https://boto3.amazonaws.com/v1/documentation/api/latest/guide/s3-example-creating-buckets.html

2. Upload file in the S3 bucket \
https://boto3.amazonaws.com/v1/documentation/api/latest/guide/s3-uploading-files.html

3. Download file from the S3 bucket \
https://boto3.amazonaws.com/v1/documentation/api/latest/guide/s3-example-download-file.html

4. Delete file from S3 bucket \
https://predictivehacks.com/?all-tips=how-to-delete-an-s3-object

5. Delete the S3 bucket \
https://dheeraj3choudhary.com/listcreate-and-delete-s3-buckets-using-python-boto3-script

# Challenges / Roadblocks encountered 
1. Having to figure out the where to get the access key id, secret access key, permissions, policies in order to access the CRUD operations in S3 bucket
2. To call the create_bucket() function, need to specify 2 arguments -- bucket_name, region for it to work
