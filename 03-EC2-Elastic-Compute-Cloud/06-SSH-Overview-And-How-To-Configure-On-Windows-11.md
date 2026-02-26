# SSH Overview and How to Configure on Windows 11

## What Is SSH?

SSH (Secure Shell) is a protocol used to securely connect to a remote
Linux server (like an EC2 instance).

Default Port: 22 (TCP)

------------------------------------------------------------------------

## Step 1: Check If SSH Is Installed

Open PowerShell and run:

ssh -V

If a version appears, SSH is installed.

If not: Settings → Apps → Optional Features → Install OpenSSH Client

------------------------------------------------------------------------

## Step 2: Use Your Key Pair (.pem)

Download your EC2 key pair file (example: mykey.pem) Place it in a
simple folder like:

C:`\Users`{=tex}`\YourName`{=tex}`\Downloads`{=tex}

------------------------------------------------------------------------

## Step 3: Set Correct Permissions

In PowerShell (inside the folder):

icacls mykey.pem /inheritance:r icacls mykey.pem /grant:r "%username%:R"

------------------------------------------------------------------------

## Step 4: Connect to EC2

For Amazon Linux:

ssh -i mykey.pem ec2-user@PUBLIC-IP

For Ubuntu:

ssh -i mykey.pem ubuntu@PUBLIC-IP

Replace PUBLIC-IP with your EC2 public IP address.

------------------------------------------------------------------------

## Important

-   Port 22 must be open in Security Group.
-   Use correct username depending on AMI.
-   Keep your .pem file secure.

------------------------------------------------------------------------

## Summary

SSH allows secure remote access to EC2 instances using a key pair.
Windows 11 has built-in SSH support.
