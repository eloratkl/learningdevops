# Task 1A: To deploy a static HTML page which a user can access

s3 bucket: http://demowebsite-task1.s3-website-ap-southeast-1.amazonaws.com/

Here are some of the steps that I've taken to complete this task.
1. Created a simple to-do-list with HTML, minimal CSS and some javascript with the aid of an online tutorial from CodeDuck.
2. Created a S3 bucket to upload the resources of my TO-DO-LIST page (task1.html, style.css, main.js, errorpage.html, errorstyle.css).
https://codepen.io/yexx/pen/XPZpoK

3. Enabled static website hosting, allowing public access to the bucket and updating the bucket policy to allow read access to everyone.
https://docs.aws.amazon.com/AmazonS3/latest/userguide/EnableWebsiteHosting.html
https://docs.aws.amazon.com/AmazonS3/latest/userguide/HostingWebsiteOnS3Setup.html

4. Created a cloudfront distribution to enable files hosted on S3 to be served effciently.
5. Enabled HTTPS with AWS Certificate Manager
https://www.stormit.cloud/blog/setup-an-amazon-cloudfront-distribution-with-ssl-custom-domain-and-s3/

# Challenges/Roadblocks encountered in Task 1A

1. Figuring out what are the pre-requisites for each step within the task
2. Unable to redeem a free domain under freenom and other free domain services. Hence, did not pursue the route 53 path of registering domain, configuring route 53 for DNS(domain name system) service
3. Dilemma on what is needed and also weighing the free and paid options
4. Had trouble linking the architecture together

# Reflection Questions in Task 1A
1. What is a cache? How does it work?
A cache is a high-speed data storage layer which stores data which is transient in nature for the purposes of serving it faster compared to accessing data's primary storage location when future requests for said data is received. The data in a cache is generally stored in fast access hardware such as RAM(Random-Access Memory), and may be used in correlation with a software component. The primary purpose of cache is to increase data retrieval performance by reducing the need to access the underlying slower storage layer.

2. What is an edge location? 
Edge locations are AWS data centers designed to deliver services with the lowest latency possible. Amazon has dozens of these data centers spread across the world.

3. What is Amazon CloudFront? How does it work?
It is a web service (content delivery netowrk) that speeds up distribution of your static and dynamic web content such as .html, .css, .js and image files to your users. It delivers your content through a worldwide network of data centers called edge locations. When a user requests content that you're serving with CloudFront, the request is routed to the edge location that provides the lowest latency(time delay), so that content is delivered with the best possible performance.

4. What is a distribution? What does it do?
5. What is the overarching term for S3, Cloudfront services?
6. What are the differences between S3 and Cloudfront? What are the benefits that Cloudfront have that makes it better than solely relying on S3?
Amazon CloudFront and Amazon S3 are primarily classified as "Content Delivery Network" and "Cloud Storage" tools respectively.Amazon Simple Storage Service (S3) is an online data storage product; admins can upload files to S3 and receive a unique URL for each file. While easy to use and inexpensive, it's not always the fastest for retrieving stored files.Amazon CloudFront works with S3 but copies files from S3 to the outer "edge" of Amazon's servers, allowing for fast retrieval.CloudFront gives you a unique URL for stored files that not only points to a single copy of your file, but also stores the file redundantly in multiple geographic locations. Amazon's systems point the URL to the closest location based on each client's browser, which can accelerate the downloading experience. CloudFront also includes additional features for fast streaming of audio and video, which makes it an excellent choice for online multimedia companies.
