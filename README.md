# Launch Your First Amazon EC2 Instance

## Objective
Deploy a virtual machine on AWS using Amazon EC2 and connect to it via SSH.

---

## Prerequisites
- AWS Account
- Basic knowledge of terminal (Git Bash / Linux)
- Internet connection

---

## Step 1: Login to AWS
1. Go to https://aws.amazon.com/
2. Click **Sign In → AWS Management Console**
3. Enter your credentials

---

## Step 2: Open EC2 Dashboard
1. Search for **EC2** in the top search bar
2. Click on **EC2 Dashboard**

---

## Step 3: Launch Instance
1. Click **Launch Instance**
2. Enter instance name (e.g., `MyFirstServer`)

---

## Step 4: Choose AMI (Operating System)
- Select **Amazon Linux 2 AMI (Free tier eligible)**

---

## Step 5: Choose Instance Type
- Select **t2.micro (Free tier eligible)**

---

## Step 6: Create Key Pair
1. Click **Create new key pair**
2. Name: `my-key`
3. Type: RSA
4. Format: `.pem`
5. Download and store it securely

---

## Step 7: Configure Security Group
- Allow:
  - SSH (Port 22) → My IP

---

## Step 8: Launch Instance
1. Click **Launch Instance**
2. Wait for initialization
3. Click **View Instance**

---


<img width="1920" height="1080" alt="Screenshot (24)" src="https://github.com/user-attachments/assets/1d939740-2802-4f6c-a81e-0bcf58258ae9" />

<img width="1920" height="1080" alt="Screenshot (25)" src="https://github.com/user-attachments/assets/d1453b40-7264-4cba-8644-63053e7a70ad" />

<img width="1920" height="1080" alt="Screenshot (26)" src="https://github.com/user-attachments/assets/be930f08-1685-4d95-b473-994d39e01bec" />

<img width="1920" height="1080" alt="Screenshot (27)" src="https://github.com/user-attachments/assets/bac5681d-c734-4ad9-bd14-999b2a55ac51" />

<img width="1920" height="1080" alt="Screenshot (29)" src="https://github.com/user-attachments/assets/dbdb49d6-81c6-47c4-923c-34b5f295c3a3" />






