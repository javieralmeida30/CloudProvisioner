#The Terraform/variables.tf code is commented out to prevent execution in GitHub Actions#

Infrastructure as Code with Terraform

This repository contains the infrastructure-as-code (IaC) code used to deploy and manage cloud infrastructure using Terraform. With Terraform, we can describe and version our infrastructure declaratively, allowing us to have precise control over our cloud resources.

Repository Structure
The repository is organized as follows:

├── .github
│   └── workflows
│       └── pipeline.yml

├── terraform
│   ├── main.tf
│   ├── variables.tf

│── .env

└── README.md



The .github/workflows directory contains the pipeline.yml file, which defines the GitHub Actions workflow used to automate the deployment and management of the infrastructure.

The terraform directory contains the main Terraform files:

main.tf: Defines the AWS resources used, such as EC2 instances, security groups, etc.

variables.tf: Defines the variables used in the Terraform code, such as the AWS region, instance type, etc.

.env: Environment file that contains sensitive configuration variables, such as AWS credentials.

Usage

Clone this repository to your local machine.

Configure the necessary variables in the .env file according to your AWS credentials and configuration.

Run the following command to initialize Terraform:

Important Notes

Keep your credentials and configuration variables confidential and do not publicly share them.

Before making significant changes, make sure you understand the impact they will have on the existing infrastructure and perform thorough testing.
