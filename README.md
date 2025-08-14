**Serverless Image Processing with S3 and Lambda**

## Table of Content

- [Solution Overview](#solution-overview)
- [Architecture Diagram](#architecture-diagram)




# Solution Overview


**Description**

Create a serverless image processing application where users upload images to an S3 bucket, triggering an AWS Lambda function that processes and resizes the images before storing them in another S3 bucket.

**Key AWS Services Used**

Amazon S3: Stores original and processed images.
AWS Lambda: Executes image processing (resize, watermarking).
Amazon DynamoDB: Store metadata about uploaded images.

# Architecture Diagram

![Architecture Diagram](<img width="1497" height="680" alt="image" src="https://github.com/user-attachments/assets/3f0d7c41-d716-4ace-b0f1-f3be9c980e18" />)


