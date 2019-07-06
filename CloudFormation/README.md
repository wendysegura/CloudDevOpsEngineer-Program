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

You can go to your aws console you should have something like screenshot below:
<img src="https://github.com/wendysegura/CloudDevOpsEngineer-Program/blob/master/CloudFormation/Images/stacks.png" width="400" height="500"> 

To view your website click on Exports and then click on link next to **DNSName-Link** like screenshot below:
<img src="https://github.com/wendysegura/CloudDevOpsEngineer-Program/blob/master/CloudFormation/Images/Exports.png" width="600" height="800"> 

# Udacity Project Architecture
<img src="https://github.com/wendysegura/CloudDevOpsEngineer-Program/blob/master/CloudFormation/Images/Udacity-Infrastructure.jpg" width="900" height="600"> 





