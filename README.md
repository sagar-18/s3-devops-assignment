# s3-devops-assignment
Transferring Files Across AWS S3 Buckets in Different AWS Accounts Using Scripting

Step 1: Create source AWS Account (name: “AS”) and S3 Bucket (name: “same-cb-bucket-sagar” )

<img width="902" alt="Screenshot 2023-07-30 at 8 03 51 PM" src="https://github.com/sagar-18/s3-devops-assignment/assets/36581523/85bc3db5-4207-4bd8-8389-f8e404eaf0c1">

Step 2: Create destination AWS Account (DG) and S3 Bucket (name: “same-cb-bucket-sagar-dest”)

<img width="917" alt="Screenshot 2023-07-30 at 8 04 21 PM" src="https://github.com/sagar-18/s3-devops-assignment/assets/36581523/53a7b1fb-28e0-4795-8719-dd43fd38f28a">

Step 3: Configure IAM Roles (name: “s3-role-cb-src-as”) and Policies (name: “s3-cb-policy-lambda-sagar”) in the source AWS account.

<img width="949" alt="Screenshot 2023-07-30 at 8 05 16 PM" src="https://github.com/sagar-18/s3-devops-assignment/assets/36581523/87ecabaa-a220-4475-a02c-35fbf5c9dce0">

<img width="990" alt="Screenshot 2023-07-30 at 8 25 29 PM" src="https://github.com/sagar-18/s3-devops-assignment/assets/36581523/8d3839e8-b7b7-42df-a26a-af38cbadd7ef">

Step 4: Create Lambda Function (name: “s3-cb-lmbda”) and add the S3 trigger in the Source AWS account.

<img width="1007" alt="Screenshot 2023-07-30 at 8 25 56 PM" src="https://github.com/sagar-18/s3-devops-assignment/assets/36581523/67e82dfe-627d-4fbe-8df6-9b5cac1e0381">

Code Used (NodeJs and Also Python boto3):

<img width="968" alt="Screenshot 2023-07-30 at 8 26 12 PM" src="https://github.com/sagar-18/s3-devops-assignment/assets/36581523/32e53df1-b49b-4621-b891-d88420987a0f">

<img width="1054" alt="Screenshot 2023-07-30 at 8 26 24 PM" src="https://github.com/sagar-18/s3-devops-assignment/assets/36581523/0ab0acb7-9adf-49ed-8adc-03d12ed67edf">

<img width="1053" alt="Screenshot 2023-07-30 at 8 26 37 PM" src="https://github.com/sagar-18/s3-devops-assignment/assets/36581523/1a561097-7108-45f4-9711-068b6a4b3888">

Python:

<img width="886" alt="Screenshot 2023-07-30 at 8 26 59 PM" src="https://github.com/sagar-18/s3-devops-assignment/assets/36581523/f5159fb8-dfe8-4276-b55f-490dc1544305">

Step 5: Add Bucket Policy in the destination S3 Bucket (name: “same-cb-bucket-sagar-dest”):

<img width="824" alt="Screenshot 2023-07-30 at 8 27 19 PM" src="https://github.com/sagar-18/s3-devops-assignment/assets/36581523/23f5b194-b55e-4a90-903e-8f8727e9bcbb">

Step 6: Test the Function by uploading any file to source AWS bucket: 
File to be uploaded: leadsquared.png

<img width="754" alt="Screenshot 2023-07-30 at 8 27 45 PM" src="https://github.com/sagar-18/s3-devops-assignment/assets/36581523/e2aefccd-d7b8-4b0f-b9a5-6d9da20eb8fb">

Step 7: Now verify in the destination bucket.

<img width="818" alt="Screenshot 2023-07-30 at 8 28 09 PM" src="https://github.com/sagar-18/s3-devops-assignment/assets/36581523/f0bf9a76-2c70-4f3a-9f6f-ab0707defbd5">

Conclusion:

In this assignment, we transferred S3 bucket data from a source AWS account to a destination AWS account's S3 bucket using a Lambda trigger function. The process involved:
  ● Setting up the necessary AWS resources.
  ● Configuring IAM roles and policies.
  ● Creating a Lambda function.
  ● Testing the functionality.

This assignment has provided hands-on experience working with AWS services, IAM roles, Lambda functions, and S3 buckets. It has showcased the power and flexibility of AWS to automate data transfer tasks and securely manage resources across different AWS accounts.




