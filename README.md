# Learn Terraform - Provision an EKS Cluster

This repo is a companion repo to the [Provision an EKS Cluster learn guide](https://learn.hashicorp.com/terraform/kubernetes/provision-eks-cluster), containing
Terraform configuration files to provision an EKS cluster on AWS.






1. create the ec2 
create the iam --> roles -> create a role
(ec2)--> next permossion --> AdministratorAccess(next tags)
Roll name (terraform-eks) --> create a role
alltach to ec2
goto action (security )modify iam role


************ aws kubectl install ******
--> (https://docs.aws.amazon.com/eks/latest/userguide/install-kubectl.html)
--> (curl -o kubectl https://amazon-eks.s3.us-west-2.amazonaws.com/1.21.2/2021-07-05/bin/darwin/amd64/kubectl)
--> ls -ltr (o/p:kubectl)

-- > change the permission ::chmod 755 kubectl
--> move the file : mv kubectl /usr/local/bin


*********download terraform*****
--> https://www.terraform.io/downloads.html
--> select the os (Ex : Linux)
--> terraform : wget https://releases.hashicorp.com/terraform/1.0.8/terraform_1.0.8_linux_amd64.zip
--> unzip the file :unzip terraform_1.0.8_linux_amd64.zip
--> delete the zip file :: rm -rf terraform_1.0.8_linux_amd64.zip 
--> move the file ::mv terraform /usr/local/bin/
--> to check the terraform version :: terraform --version(Terraform v1.0.8 on linux_amd64)
Set up and initialize your Terraform workspace
---> yum install git -y
https://github.com/ANJINAYULU/cluster.git