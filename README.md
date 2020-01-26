# terraform-jenkins
Provisioning Jenkins server using Terraform “Infrastructure as a code” principle.
# Jenkins Install in EC2 Instance


## Usage

```hcl
module "ec2_instance" {
  region        = "us-west-2"
  key-name      = "ec2-terraform-jenkins"
  instance_type = "t2.micro"

}
```

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| region | AWS region | string | us-east-1 | yes |
| key-name | ec2 access key name | string | yes |
| instance_type | ec2 instance_type | string | t2.micro | yes |
