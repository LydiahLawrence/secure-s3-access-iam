# Secure File Upload & Access in Amazon S3 using IAM

This project simulates a real-world use case where a business needs to allow limited access to upload and read files in Amazon S3 — while restricting actions like deletion. It also includes a simulation of access denial and how to troubleshoot IAM permission errors.

## What I Set Out to Build

I wanted to create a secure environment in S3 where only specific users could upload and read files. This is common in companies managing client documents, logs, reports, or internal files.

My goal was to:
- Create a private S3 bucket
- Write a custom IAM policy allowing `PutObject`, `GetObject`, and `ListBucket`
- Test access from a restricted IAM user
- Simulate a permissions error by removing `PutObject` from the policy
- Use versioning and lifecycle rules to manage data

## Services & Tools Used

- Amazon S3
- AWS IAM (Users, Groups, Policies)
- AWS CLI
- Lifecycle Rules & Versioning
- Kali Linux (for CLI testing)

## What I Built

- Private S3 bucket with object ownership enforced
- Versioning enabled to protect files
- Lifecycle rule to delete files after 30 days
- IAM user group with limited access policy
- Test IAM user with CLI access to simulate uploads
- Simulated "Access Denied" error and resolved it

## screenshots uploaded

- S3 bucket setup
- IAM policy creation
- Successful file upload via CLI
- Denied upload after removing permission
- Lifecycle rule and versioning

## 🧠 Key Concepts Practiced

- IAM access control and least-privilege policy design
- Testing permissions from a non-root user
- S3 lifecycle and versioning strategies
- Troubleshooting permissions errors in AWS

## 🔗 Live Blog Post

You can read the full reflection and write-up of this project on my website:  
[cloudwithlydiah.com]
