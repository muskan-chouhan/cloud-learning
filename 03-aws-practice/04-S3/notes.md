# Amazon S3 (Simple Storage Service)

## What is Amazon S3?

Amazon S3 (Simple Storage Service) is an AWS Object Storage service used to store and retrieve any amount of data from anywhere over the internet.

It is designed for:
- High Durability
- High Availability
- Scalability
- Secure Storage

---

# Why do we need S3?

Before Cloud:

- Files were stored on local servers.
- Storage had limited capacity.
- Hardware failures could cause data loss.
- Scaling storage was difficult.

AWS introduced S3 to provide highly scalable and durable object storage.

---

# What can we store in S3?

- Images
- Videos
- Documents
- PDF Files
- Audio Files
- Backup Files
- Static Website Files
- Application Assets

---

# What is a Bucket?

A Bucket is a container used to store objects in Amazon S3.

Example:

Bucket Name:
my-first-bucket

---

# What is an Object?

An Object is a file stored inside an S3 bucket.

Every object contains:

- File Data
- Object Key (File Name)
- Metadata

Example:

Bucket:
my-first-bucket

Objects:

logo.png

resume.pdf

video.mp4

---

# Object Key

The unique name of an object inside a bucket.

Example:

images/profile.png

documents/resume.pdf

---

# Features of Amazon S3

- Object Storage
- Highly Scalable
- Highly Durable (11 9's durability)
- High Availability
- Secure Storage
- Versioning
- Encryption
- Static Website Hosting

---

# Storage Classes

We discussed:

- S3 Standard
- S3 Intelligent-Tiering
- S3 Standard-IA
- S3 One Zone-IA
- Glacier Instant Retrieval
- Glacier Flexible Retrieval
- Glacier Deep Archive

---

# Versioning

Versioning allows multiple versions of the same object.

Benefits:

- Recover deleted files
- Recover overwritten files
- Maintain file history

---

# Encryption

Encryption protects data stored in S3.

It converts readable data into encrypted data.

---

# Static Website Hosting

Amazon S3 can host static websites.

Static websites contain:

- HTML
- CSS
- JavaScript

No backend code is executed.

---

# Pre-Signed URL

A Pre-Signed URL allows temporary access to upload or download an object from S3.

Benefits:

- Secure
- Time-limited
- No AWS credentials shared

---

# Difference between S3 and EBS

| Amazon S3 | Amazon EBS |
|------------|------------|
| Object Storage | Block Storage |
| Stores files | Stores disk blocks |
| Accessible over Internet | Attached to EC2 |
| Highly Scalable | Fixed Volume Size |
| Used for Images, Videos, Backups | Used as EC2 Disk |

---

# Real World Use Cases

- Image Storage
- Video Storage
- Website Assets
- Static Website Hosting
- Application Backups
- Log Storage
- Resume Storage
- User Uploads

---

# Practical Performed

✅ Created S3 Bucket

✅ Uploaded Files

✅ Enabled Static Website Hosting

✅ Hosted Static Website

✅ Generated Pre-Signed URL

---

# Interview Questions

Q1. What is Amazon S3?

Q2. What is a Bucket?

Q3. What is an Object?

Q4. What is an Object Key?

Q5. Difference between S3 and EBS?

Q6. What is Versioning?

Q7. What is Static Website Hosting?

Q8. What is a Pre-Signed URL?

---

# Notes

Amazon S3 is an Object Storage service.

It is commonly used for:

- File Storage
- Static Website Hosting
- User Uploads
- Application Assets
- Backup Storage
