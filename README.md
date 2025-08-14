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
3. Each object contains (key, value, metadata, version ID, access control information).  
4. Virtually **unlimited storage** (You can store data as needed, without worrying about limits).  
5. You can create up to **100 buckets per account** (by default).  
6. Each bucket must have a globally **unique name** (Because bucket names are part of the public URL if used for hosting or accessing objects via HTTP).  
7. Maximum object size is **5 TB**  
   - But for uploads larger than 5 GB, AWS recommends using multipart upload for better performance and reliability.  
   - To upload a file larger than 160 GB, use the AWS CLI, AWS SDKs, or Amazon S3 REST API.  
