# AWS_Cloud_Travel_Website_deployment
This project demonstrates how to host a static website using Amazon Web Services (AWS). It covers steps from setting up an S3 bucket, configuring CloudFront and hosting website on bucket URL.

-----------------------------------------------------------------------------------------------------------------------------------------------------

# Architecture 
<img width="447" height="437" alt="image" src="https://github.com/user-attachments/assets/6e87b5a3-9fc5-4563-ae13-0af430e47fe1" />



---------------------------------------------------------------------------------------------------------------------------------------------------------

# Prerequisites 

* An AWS account
* Website source files (`index.html`, `style.css`, `script.js`, etc.)

-----------------------------------------------------------------------------------------------------------------------------------------------------------

# Steps to Deploy 

1. Create an S3 Bucket

* Go to the "S3 Console" → Create bucket
* Name the bucket (e.g., `my-bucketId`)
* Disable “Block all public access”
* Enable Static Website Hosting under the bucket’s "Properties"
* Note the "endpoint URL"

2. Upload Your Website Files

* Use AWS CLI or Console to upload files
< index.html , css files , vendor >


3. Configure Bucket Policy

* Allow public read access
* Host website using "index.html"


4. Setup CloudFront

* Go to "CloudFront" → Create distribution
* Set "Origin Domain" to your S3 bucket
* Enable "Redirect HTTP to HTTPS" for security
* Copy the "CloudFront Domain Name" — this becomes your website URL

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Testing

* Bucket Web endpoint - s3-website-us-east-1.amazonaws.com

* CloudFront - cloudfront.net

* S3 bucket object - amazonaws.com/index.html

---------------------------------------------------------------------------------------------------------------------------------------------------------------------
