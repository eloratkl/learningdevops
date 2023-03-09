# Task 1: To deploy a static HTML page which a user can access

s3 bucket: http://demowebsite-task1.s3-website-ap-southeast-1.amazonaws.com/

cloudfront: https://d2fj33c3isd9xv.cloudfront.net/

Here are some of the steps that I've taken to complete this task.
1. Created a simple to-do-list with HTML, minimal CSS and some javascript with the aid of an online tutorial from CodeDuck.
2. Created a S3 bucket to upload the resources of my TO-DO-LIST page (task1.html, style.css, main.js).
3. Enabled static website hosting, allowing public access to the bucket and updating the bucket policy to allow read access to everyone.
4. Created a cloudfront distribution to enable files hosted on S3 to be served effciently.
5. Enabled HTTPS with AWS Certificate Manager

# Challenges/Roadblocks encountered in Task 1

1. Figuring out what are the pre-requisites for each step within the task
2. Unable to redeem a free domain under freenom and other free domain services. Hence, did not pursue the route 53 path of registering domain, configuring route 53 for DNS(domain name system) service
3. Dilemma on what is needed and also weighing the free and paid options
4. Had trouble linking the architecture together
