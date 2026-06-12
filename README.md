# AWS Infrastructure Automation with Terraform

This project demonstrates how to automate the deployment and management of cloud infrastructure on AWS using Terraform as Infrastructure as Code (IaC). In this project, a production-ready AWS S3 Bucket is provisioned automatically.

## 📺 Infrastructure Deployment & Verification Video
Click the link below to watch the live step-by-step infrastructure provisioning and verification:
👉 [Watch the Terraform AWS S3 Deployment on Google Drive](https://drive.google.com/file/d/1xmPqW5rb2bij21v5ZhCQ1Iia0BMzQvZ1/view?usp=sharing)

## 🚀 Architecture Overview
- **Infrastructure as Code (IaC):** Terraform (v1.15+)
- **Cloud Provider:** Amazon Web Services (AWS)
- **Core Resource:** AWS S3 Bucket (`prod_assets_bucket`)
- **Region:** `eu-north-1` (Stockholm)

## 🛠️ Prerequisites & Tools Used
- **OS:** Windows 11
- **Terraform** v1.15.6
- **AWS CLI** v2.35.3
- **VS Code** with HashiCorp Terraform extension

## 💻 How to Run This Project Locally

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/eng-imonmahmud/aws-infrastructure-automation.git](https://github.com/eng-imonmahmud/aws-infrastructure-automation.git)
   cd aws-infrastructure-automation
2. Configure AWS Credentials: aws configure
3. Initialize Terraform: terraform init
4. Review the Execution Plan: terraform plan
5. Deploy Infrastructure to AWS: terraform apply
6. Clean Up Resources (To avoid billing): terraform destroy

🔒 Security Best Practices Implemented
IAM User Principle: Avoided using root accounts; deployed via a dedicated IAM user (terraform-user) with restricted programmatic access.

Git Protection: Used .gitignore to ensure state files (.tfstate) and sensitive local backend caches are never exposed publicly.
