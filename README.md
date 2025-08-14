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

** Amazon S3
Amazon S3:
✅ Amazon S3 stands for Simple Storage Service.
✅S3 stores data as 𝐨𝐛𝐣𝐞𝐜𝐭𝐬.
✅ Each object contains (key-value- Metadata-version ID -access control information).
✅Virtually 𝐮𝐧𝐥𝐢𝐦𝐢𝐭𝐞𝐝 𝐬𝐭𝐨𝐫𝐚𝐠𝐞 (You can store data as needed, without worrying about limits).
✅You can create up to 𝟏𝟎𝟎 𝐛𝐮𝐜𝐤𝐞𝐭𝐬 per account (by default).
✅Each bucket must have a globally 𝐮𝐧𝐢𝐪𝐮𝐞 𝐧𝐚𝐦𝐞(Because bucket names are part of the public URL if used for hosting or accessing objects via HTTP).
✅Maximum object size is 𝟓 𝐓𝐁
- (But for uploads larger than 5 GB, AWS recommends using multipart upload for better performance and reliability)
- (To upload a file larger than 160GB, use the AWS CLI, AWS SDKs or Amazon S3 REST API)
