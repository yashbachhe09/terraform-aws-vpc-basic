# terraform-aws-vpc-basic

A basic Terraform module that creates a VPC, Subnet, and EC2 instance in AWS.

## Usage

```hcl
module "vpc_basic" {
  source         = "github.com/<your-github-username>/terraform-aws-vpc-basic"
  region         = "us-east-1"
  vpc_cidr       = "10.0.0.0/16"
  subnet_cidr    = "10.0.1.0/24"
  ami_id         = "ami-1234567890abcdef0"
  instance_type  = "t2.micro"
}
