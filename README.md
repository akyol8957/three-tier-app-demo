# three-tier-app-demo

Gathering Information
Step 0 
	1. Get VPC CIDR block from Networking Team. 
	2. Get DB Instance From Database Team  Or Build it on Step7
	3. Get AMI from Software team   or Build it with Packer 



Building Infrastructure
Step1. 

Environment Preparation
Create s3 bucket   
Name: project-bucket123
        Ø  add versioning 
        Ø  add encryption
        Ø  tags 

Step2 
Setup  SCM
URL: git@github.com:farrukh90/three-tier-app-demo.git
Visibility: Private


Step3
Configure infrastructure  (VPC)
1. Create neseccary variable
2. configure S3 backend
3. download public module   or    author module from scratch


Step4 
Build VPC 
1. Build VPC
2. Get output VPC











Application Deployment
Step5
Build Auto Scaling group
1. Download public repo for AWS ASG
2. Configure backend    to store  tfstate
3. Get output 
4. Read Remote VPC Information  (terraform_remote_state)



Step6
Configure LB on public Subnet
1. Build LB
2. Attach LB to ASG 
3. Add neseccary 





Database Team 
Step7
1. Get Public Module 
2. Configure backend
3. Get output 
4. Read Remote VPC Information  (terraform_remote_state)
5. Build Security Group









Automation with Jenkins 
Purpose 
	1. Keep track of resources 
	2. Easier configuration management 
Change Approval 