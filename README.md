# Terraform AWS Infrastructure Project

This project provisions AWS infrastructure using Terraform.

## Resources Created

- EC2 Instance
- Security Group
- S3 Bucket

## Project Structure

```bash
.
├── main.tf
├── outputs.tf
├── variables.tf
├── .gitignore
└── README.md
```

## Prerequisites

Install:

- Terraform
- AWS CLI
- Git

Configure AWS credentials:

```bash
aws configure
```

## Terraform Commands

Initialize Terraform:

```bash
terraform init
```

Validate configuration:

```bash
terraform validate
```

Preview infrastructure changes:

```bash
terraform plan
```

Apply infrastructure:

```bash
terraform apply
```

Destroy infrastructure:

```bash
terraform destroy
```

## AWS Resources

### EC2 Instance

- Instance Type: t3.medium
- Region: ap-south-2
- Security Group:
  - SSH Port 22
  - HTTP Port 80

### S3 Bucket

Globally unique S3 bucket created using Terraform.

## Outputs

Terraform outputs:

- EC2 Public IP
- S3 Bucket Name

View outputs:

```bash
terraform output
```

## Important Notes

Do not commit:

- `.terraform/`
- `terraform.tfstate`
- `.pem` files
- AWS secrets

## Git Ignore

The `.gitignore` file excludes Terraform cache, state files, and sensitive files.
