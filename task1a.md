# Task 1A: To deploy a static HTML page which a user can access

s3 bucket: http://demowebsite-task1.s3-website-ap-southeast-1.amazonaws.com/

cloudfront: https://d2fj33c3isd9xv.cloudfront.net/

Here are some of the steps that I've taken to complete this task.
1. Created a simple to-do-list with HTML, minimal CSS and some javascript with the aid of an online tutorial from CodeDuck.
2. Created a S3 bucket to upload the resources of my TO-DO-LIST page (task1.html, style.css, main.js).
3. Enabled static website hosting, allowing public access to the bucket and updating the bucket policy to allow read access to everyone.
https://docs.aws.amazon.com/AmazonS3/latest/userguide/EnableWebsiteHosting.html
https://docs.aws.amazon.com/AmazonS3/latest/userguide/HostingWebsiteOnS3Setup.html

4. Created a cloudfront distribution to enable files hosted on S3 to be served effciently.
5. Enabled HTTPS with AWS Certificate Manager
https://www.stormit.cloud/blog/setup-an-amazon-cloudfront-distribution-with-ssl-custom-domain-and-s3/

# Challenges/Roadblocks encountered in Task 1

1. Figuring out what are the pre-requisites for each step within the task
2. Unable to redeem a free domain under freenom and other free domain services. Hence, did not pursue the route 53 path of registering domain, configuring route 53 for DNS(domain name system) service
3. Dilemma on what is needed and also weighing the free and paid options
4. Had trouble linking the architecture together

# Reflection Questions in Task 1
1. What is a cache?
2. What is an edge location?
3. What is a distribution? What does it do?
4. What is the overarching term for S3, Cloudfront services?
5. What are the differences between S3 and Cloudfront? What are the benefits that Cloudfront have that makes it better than solely relying on S3?