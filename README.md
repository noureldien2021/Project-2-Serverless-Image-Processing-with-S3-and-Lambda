## Serverless Image Processing with S3 and Lambda

## Table of Content
- [Solution Overview](#solution-overview)
- [Architecture Diagram](#architecture-diagram)
- [AWS Services Used](#aws-services-used)
  - [Amazon S3](#amazon-s3)
  - [AWS Lambda](#aws-lambda)
  - [Amazon DynamoDB](#amazon-dynamodb)
 




# Solution Overview

**Description**
Create a serverless image processing application where users upload images to an S3 bucket, triggering an AWS Lambda function that processes and resizes the images before storing them in another S3 bucket.

**Key AWS Services Used**
Amazon S3: Stores original and processed images.
AWS Lambda: Executes image processing (resize, watermarking).
Amazon DynamoDB: Store metadata about uploaded images.

# Architecture Diagram

![Architecture Diagram](https://github.com/noureldien2021/Project-2-Serverless-Image-Processing-with-S3-and-Lambda/blob/main/_Serverless%20Image%20Processing.jpeg?raw=true)

# AWS Services Used

**Amazon S3**

1. Amazon S3 stands for Simple Storage Service.  
2. S3 stores data as **objects**.  
3. SSE-S3 (Server-Side Encryption) → AWS manages the keys (default option).
4. In this project, S3 stores both **original uploaded images** and **processed images** in separate buckets.
5. S3 integrates seamlessly with Lambda to **trigger image processing automatically** when a new file is uploaded.

**AWS Lambda**

1. AWS Lambda is a **serverless compute service** that runs your code without provisioning or managing servers.
2. In this project, Lambda is **triggered automatically** when a new image is uploaded to the S3 bucket.
3. It performs **image processing tasks** such as resizing and watermarking.

**Amazon DynamoDB**
1. Amazon DynamoDB is a **fully managed NoSQL database** that provides fast and predictable performance.
2. In this project, DynamoDB is used to **store metadata** about uploaded images (e.g., filename, size, timestamp).
   

 
