# Terraform with AWS 3 tire arc

A template and configuration that reuses modules from the terraform registry to
create a three tier VPC and deploy a sample app to it, where:

The public presentation tier is an nginx web server


The private application tier hosts a spring boot application that persists data
in the DB tier.

The db tier hosts an RDS mysql.



Take a copy of terraform.tfvars.template and substitute required values.
process

terraform init
terraform validate
terraform plan
terraform apply -var-file=terraform.tfvars


