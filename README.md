# AWS Cloud Resume Challenge
### Project Overview
This repository contains the code and documentation for the Cloud Resume Challenge, a personal resume project that is deployed on AWS using a full cloud-native stack. The challenge showcases my skills in cloud computing, infrastructure as code (IaC), and serverless architecture.

### Challenge Components
The Cloud Resume Challenge consists of multiple parts:

1. HTML/CSS: My resume is written in HTML and styled with CSS. The resume is hosted on AWS and can be accessed via a custom domain.
2. S3 and CloudFront: The resume is deployed on an AWS S3 bucket, which serves the static files. CloudFront is used as a content delivery network (CDN) to ensure fast and secure delivery of the resume globally.
3. DNS via Route 53: A custom domain is managed via AWS Route 53, and the site is accessible using HTTPS.
4. Visitor Counter (JavaScript + API Gateway + Lambda + DynamoDB): A visitor counter on the resume page shows how many people have visited the site. It uses JavaScript to fetch data from a serverless API, which interacts with AWS Lambda and DynamoDB to store the count.
5. Infrastructure as Code (IaC) with Terraform: The entire infrastructure, including S3, CloudFront, Route 53, Lambda, DynamoDB, and API Gateway, is provisioned using Terraform.
6. CI/CD with GitHub Actions: The project uses GitHub Actions to automate deployments and updates to the resume and infrastructure. Whenever changes are pushed to the repository, the CI/CD pipeline automatically updates the resources in AWS.

### Project Features
- Static Resume Hosting: My resume is written in HTML and styled with CSS, hosted on an S3 bucket, and distributed through CloudFront.
- HTTPS via AWS Certificate Manager: Secure connections are ensured by configuring HTTPS with a certificate managed through AWS Certificate Manager (ACM).
- Serverless Visitor Counter: Using AWS Lambda, API Gateway, and DynamoDB, the site tracks the number of visitors with a fully serverless solution.
- Infrastructure as Code: The entire project infrastructure is built and managed using Terraform. This allows for quick setup and tear-down in a consistent and repeatable manner.
- Continuous Integration & Deployment: GitHub Actions is used to automate the build and deployment of the website and its infrastructure.

### Technologies Used
**AWS Services:**
- S3
- CloudFront
- Route 53
- API Gateway
- Lambda (Node.js for backend logic)
- DynamoDB
- Certificate Manager (ACM)

**Infrastructure:**
- Terraform for IaC (Infrastructure as Code)
  
**CI/CD:**
- GitHub Actions
  
**Languages:**
- HTML, CSS (frontend)
- JavaScript (frontend and Lambda function)
- JSON (for DynamoDB interaction)

### Future Improvements
- Add more sections and style improvements to the resume.
- Implement a contact form using another serverless AWS service.
- Set up additional monitoring using CloudWatch.

### License
This project is licensed under the MIT License - see the LICENSE file for details.

### Acknowledgments
- Cloud Resume Challenge: https://cloudresumechallenge.dev/docs/the-challenge/aws/
- AWS Documentation
- Terraform Documentation
