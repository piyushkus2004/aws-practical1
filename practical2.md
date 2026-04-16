# Static Website Deployment on AWS S3

## Objective
To host a static website using Amazon S3 by enabling static website hosting and configuring public access.

---

## Prerequisites
- AWS account
- Basic HTML file (index.html)

---

## Steps to Deploy

### 1. Create an S3 Bucket
- Go to AWS Console
- Open S3 service
- Click "Create Bucket"
- Enter a unique bucket name
- Select a region
- Disable "Block all public access"
- Create the bucket

---

### 2. Upload Website Files
- Open the created bucket
- Click "Upload"
- Add your `index.html` file
- Upload the file

---

### 3. Enable Static Website Hosting
- Go to "Properties"
- Scroll to "Static website hosting"
- Click "Edit"
- Enable hosting
- Set:
  - Index document: `index.html`
- Save changes

---

### 4. Configure Bucket Policy
Go to "Permissions" → "Bucket Policy" and add:

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadAccess",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::your-bucket-name/*"
    }
  ]
}
