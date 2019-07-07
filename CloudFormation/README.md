# Deploy a High-Availability Web App using CloudFormation

Link showing it successfully works:</br>
http://serve-WebAp-11D6GNCP7035O-557630779.us-west-2.elb.amazonaws.com


## How to

### AWS Console:</br>
1) Go to services
2) Search for CloudFormation click on it
3) Now you can view the stacks you will be creating from the terminal</br>
<img src="https://github.com/wendysegura/CloudDevOpsEngineer-Program/blob/master/CloudFormation/Images/Cloudformation.png" width="500" height="400"> 


### Login to your AWS CLI 
Link on How to Set AWS CLI: https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html </br>

### On your Terminal
Open your Terminal </br>
Download Repository with Code </br>
In terminal run:</br>
`git clone git@github.com:wendysegura/CloudDevOpsEngineer-Program.git`</br>
`cd CloudDevOpsEngineer-Program/CloudFormation/`</br>

Now we can create the stacks:</br>
`./create.sh infrastructure infrastructure.yml infra_parameters.json`</br>
Once that stack has completed you can run:</br>
`./create.sh servers servers.yml server_parameters.json`</br>

You can go to your aws console you should have something like screenshot below:</br>

<img src="https://github.com/wendysegura/CloudDevOpsEngineer-Program/blob/master/CloudFormation/Images/stacks.png" width="400" height="500"> </br>

To view your website click on Exports and then click on link next to **DNSName-Link** like screenshot below:</br>

<img src="https://github.com/wendysegura/CloudDevOpsEngineer-Program/blob/master/CloudFormation/Images/Exports.png" width="500" height="400"> </br>

# Udacity Project Architecture
<img src="https://github.com/wendysegura/CloudDevOpsEngineer-Program/blob/master/CloudFormation/Images/Udacity-Infrastructure.jpg" width="900" height="600"> 


# Project Specifications for the Project (Ruberic)

### The Basics
**Parameters:** More than 1 <br /> 
**Resources:** LoadBalancer, Launch Configuration, AutoScaling group a health check, security groups and Listner and Target Group<br /> 
**Outputs:** URL with Load Balancer DNS Name and "http" in front of it.<br /> 
**Working Test:** Url to verify it works with page that reads "it works! Udagram, Udacity"<br /> 

### Load Balancer</break>
**Target Group:** The auto-scaling group needs to have a property that associates it with a target group. 
The Load Balancer will have a Listener rule associated with the same target group.</br>
**Health Check and Listener:** Port 80 should be used in Security groups, health checks and listeners associated with the load balancer<br /> 

### Auto-Scaling<br /> 
**Subnets:** Students should be using PRIV-NET ( private subnets ) for their auto-scaling instances.<br /> 
**Machine Specs:** The machine should have 10 GB or more of disk and should be a t3.small or better.<br /> 
**SSH Key:** There shouldn’t be a ‘keyname’ property in the launch config.<br /> 

### Bonus</br>
**Output:** Any values in the output section are a bonus<br />
**Bastion Host:** Any resource of type AWS::EC2::Instance, optional, but nice to have.<br />



