# Terraform code 

## Maintain vpc & eks with terraform for vprofile project
## Overview

This repository contains the Terraform code to manage the VPC and EKS infrastructure for the vProfile project. The infrastructure is defined using Terraform scripts and is maintained using GitHub Actions for continuous integration and deployment.

## Prerequisites

Ensure you have the following tools installed before proceeding:
- Terraform version 1.6.3
- AWS CLI configured with appropriate permissions

## Usage

Follow the steps below to initialize and apply the Terraform configurations:

1. **Initialize Terraform:**
    ```sh
    terraform init
    ```

2. **Format and Validate Terraform Code:**
    ```sh
    terraform fmt -check
    terraform validate
    ```

3. **Plan and Apply Terraform Configuration:**
    ```sh
    terraform plan -out planfile
    terraform apply -auto-approve -input=false -parallelism=1 planfile
    ```

## Continuous Integration and Deployment

The project uses GitHub Actions to automate the deployment process. The workflow files are located in the `.github/workflows` directory. The CI/CD pipeline includes the following steps:
- Linting and formatting checks
- Terraform validation
- Terraform plan and apply

Ensure that any changes to the Terraform code are committed and pushed to the repository to trigger the GitHub Actions workflow.


## Tools required
Terraform version 1.6.3

### Steps
* terraform init
* terraform fmt -check
* terraform validate
* terraform plan -out planfile
* terraform apply -auto-approve -input=false -parallelism=1 planfile
####
#####
