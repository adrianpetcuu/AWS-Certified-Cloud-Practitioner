# AWS Access Keys, CLI and SDK (Short Overview)

## AWS Access Keys

Access Keys are credentials used to access AWS programmatically (not
through the Console).

They consist of: - Access Key ID - Secret Access Key

They are used for: - AWS CLI - SDKs - API calls

Important: - Do NOT share them - Do NOT upload them to GitHub - Rotate
them regularly - Prefer IAM Roles when possible

------------------------------------------------------------------------

## AWS CLI (Command Line Interface)

The AWS CLI allows you to manage AWS services from the terminal.

Example: aws s3 ls

It uses Access Keys configured with: aws configure

Best for: - Automation - Scripting - DevOps tasks

------------------------------------------------------------------------

## AWS SDK

SDK (Software Development Kit) allows developers to interact with AWS
services from code.

Available for: - Python - Java - JavaScript - C# - Go - and more

Your application can upload files, create instances, or manage resources
using the SDK.

------------------------------------------------------------------------

## Best Practice

Instead of hardcoding Access Keys: - Use IAM Roles - Use temporary
credentials - Follow the Principle of Least Privilege

------------------------------------------------------------------------

## Summary

-   Access Keys = programmatic credentials
-   CLI = manage AWS from terminal
-   SDK = integrate AWS into applications
-   Always secure and rotate credentials
