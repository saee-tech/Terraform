# Terraform
Learing


# Terraform - Day 1

## Step 1: Install Terraform
Download and install Terraform from the official site.  
Verify installation: using the command below.
terraform --version
Step 2: Write the Terraform Script provider "aws" {
  region = "ap-south-1"
}

resource "aws_instance" "terr1" {
  ami           = "ami-xxxxxxxx"   # Replace with a valid AMI ID from AWS
  instance_type = "t2.micro"       # Free tier eligible
}
terraform init       # Initialise Terraform and download provider plugins
terraform validate   # Validate the configuration
terraform plan       # Preview the resources that will be created
terraform apply      # Create the resources
terraform destroy    # Delete the resources



<img width="1583" height="106" alt="image" src="https://github.com/user-attachments/assets/6b7148d9-9c35-4425-b1f1-8f3516c6c069" />
