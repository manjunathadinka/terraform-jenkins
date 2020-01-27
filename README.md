# terraform-jenkins
# Provisioning Jenkins server using Terraform “Infrastructure as a code” principle.


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
| key-name | ec2 access key name | string | ec2-terraform-jenkins | yes | 
| instance_type | ec2 instance_type | string | t2.micro | yes |



# Deploy “Your JAR/WAR” file using the CI/CD pipeline to Test.
The repository contains a simple Java application which outputs the string "Hello world!" and is accompanied by a couple of unit tests to check that the main application works as expected. The results of these tests are saved to a JUnit XML report.

The jenkins directory contains an example of the Jenkinsfile (i.e. Pipeline) you'll be creating yourself during the tutorial and the scripts subdirectory contains a shell script with commands that are executed when Jenkins processes the "Deliver" stage of the Pipeline.
