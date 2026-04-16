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
```

<img width="1920" height="1080" alt="Screenshot (37)" src="https://github.com/user-attachments/assets/49df7d97-1ba3-4a4c-b671-71d51a2d9c54" />

<img width="1920" height="1080" alt="Screenshot (38)" src="https://github.com/user-attachments/assets/61365c5f-2d4f-4d08-ba1a-a21cdc233cd2" /><img width="1920" height="1080" alt="Screenshot (39)" src="https://github.com/user-attachments/assets/6d4100f8-6905-49e2-9d5a-b9707d972552" />


<img width="1920" height="1080" alt="Screenshot (40)" src="https://github.com/user-attachments/assets/c24ddd72-0a94-4dd3-bfd1-d538bf2f6b4b" />


<img width="1920" height="1080" alt="Screenshot (41)" src="https://github.com/user-attachments/assets/3041e7fa-b8df-4477-ac8c-c8c2060414df" />



<img width="1920" height="1080" alt="Screenshot (42)" src="https://github.com/user-attachments/assets/31ef1344-3afe-4b43-8016-725fcabef3fa" />


<img width="1920" height="1080" alt="Screenshot (46)" src="https://github.com/user-attachments/assets/ac777d72-aa25-491a-978a-011d3b1e75e9" />


<img width="1920" height="1080" alt="Screenshot (47)" src="https://github.com/user-attachments/assets/98f39c7c-f85a-4d7f-adf6-53d35eab1ecc" />



<img width="1920" height="1080" alt="Screenshot (48)" src="https://github.com/user-attachments/assets/a1ec7f3a-2448-4396-b393-69b6ae3deef1" />


<img width="1920" height="1080" alt="Screenshot (49)" src="https://github.com/user-attachments/assets/4410fdc1-afba-490d-9356-b1e7be53ded8" />












