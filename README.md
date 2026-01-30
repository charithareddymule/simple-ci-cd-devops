# Simple CI/CD Pipeline – AWS Sandbox

## Project Overview
This project demonstrates a simple CI/CD pipeline using GitHub Actions.
The goal is to automatically deploy a static website to AWS S3.

## Architecture
GitHub Repository  
→ GitHub Actions (CI/CD)  
→ AWS S3 (Static Website Hosting)

## Tools & Services Used
- GitHub
- GitHub Actions
- AWS S3
- AWS IAM (sandbox environment)

## What I Implemented
- Created a GitHub repository with static website files
- Wrote a GitHub Actions workflow for automated deployment
- Configured AWS S3 for static website hosting
- Attempted IAM user creation for CI/CD authentication

## Sandbox Limitation (Important Note)
While implementing CI/CD deployment to AWS S3, IAM user creation was restricted.

The AWS sandbox account uses a temporary assumed role (voclabs),
which does not allow `iam:CreateUser` or access key generation.

This is a known limitation of AWS Academy / sandbox environments.

In a real AWS account, this pipeline would authenticate using:
- IAM user access keys, or
- IAM role with OIDC (recommended approach)

## Key Learning
- Understood CI/CD pipeline structure using GitHub Actions
- Learned how authentication works between GitHub and AWS
- Understood sandbox vs real AWS account limitations
- Gained experience in documenting technical constraints clearly
