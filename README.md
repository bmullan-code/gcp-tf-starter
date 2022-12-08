# gcp-tf-starter

Starter project for using terraform with google cloud. Uses the google provider and a terraform service account (rather than using account credentials)

## Getting started
- Create a service account and grant it the roles required for the resources you will be creating
- To get started in cloud shell 
```
gcloud auth list
gcloud config list project
export PROJECT_ID=$DEVSHELL_PROJECT_ID
```
- clone this repository
```
git clone https://github.com/bmullan-google/gcp-tf-starter
```
- Edit the terrafrom.tfvars file and replace values with your values
- run terraform with the following commands
```
# install provider and dependencies
terraform init
# verify your plan
terraform plan
# apply your plan
terraform apply --auto-approve
```
- Next steps ... review the terraform google cloud provider
https://registry.terraform.io/providers/hashicorp/google/latest/docs/guides/getting_started



