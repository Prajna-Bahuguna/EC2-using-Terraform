# EC2-using-Terraform
Configured AWS EC2 using Terraform and Nginx webserver is installed on that EC2.</br>
# Description 
This project uses Terraform which is IaaC (Infrastructure as a Code) tool which helps to build, change and version infrastructure easily and efficiently. AWS EC2 which is like a physical server to deploy our applications in aws environment is configured using Terraform and Nginx webserver is installed on that ec2 by providing commands in main.tf file which runs when EC2 boots. This project uses Terraform v1.0.10 version. </br>

# Steps to setup 
1. Export your AWS IAM Access and Secret key in your local machine using aws cli.
2. Create public and private keys on your local machine using command: "ssh-keygen -t rsa."
3. Go to main.tf file and paste your public key in "public_key" at the end of file.
4. Go to your AWS console -> search -> EC2 -> Network and Security -> keypairs -> actions -> import key-pair -> paste private key of your local machine.
5. Run the following Terraform commands:
- Terraform init -> This initializes directory, pull down providers.
- Terraform validate -> validate code for syntax.
- Terraform plan -> evaluates a Terraform configuration to determine the desired state of all the resources.
- Terraform apply -> executed the actions proposed in Terraform plan.
6. Go to your AWS console -> search -> EC2 -> EC2 is created.
7. Terrafrom destroy -> destroys all objects managed by a Terraform configuration. </br>
*Leave a star and share this if you found this helpful.*
