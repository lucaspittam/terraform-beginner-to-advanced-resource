### Important Note

Note that every region has a different AMI ID. The AMI ID's keeps on changing so make sure you use the latest AMI ID from the AWS console similar to the way it is shown in the video.

### Documentation Referred:

https://registry.terraform.io/

https://registry.terraform.io/providers/hashicorp/aws/latest/docs

### first_ec2.tf

```sh
provider "aws" {
  region     = "us-east-2"
  access_key = "AKIAWCPADDUKIJ2KQC76"
  secret_key = "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"
}

resource "aws_instance" "myec2" {
   ami = "ami-0568773882d492fc8"
   instance_type = "t2.micro"
}
```
### Commands:

```sh
terraform init
terraform plan
terraform apply
```
