# Capstone Project 1: Static Web Application Deployment

## Project Overview
This project demonstrates deploying a static web application using **AWS S3** and **CloudFront**. The workflow includes creating an S3 bucket, uploading static website files, enabling static website hosting, and serving the website via CloudFront.

---

## Steps Taken

1. Created an S3 bucket with a unique name
2. Configured bucket policy for public read access:
   ```json
   {
       "Version": "2012-10-17",
       "Statement": [
           {
               "Sid": "PublicReadGetObject",
               "Effect": "Allow",
               "Principal": "*",
               "Action": "s3:GetObject",
               "Resource": "arn:aws:s3:::my-static-webapp-2026/*"
           }
       ]
   }
