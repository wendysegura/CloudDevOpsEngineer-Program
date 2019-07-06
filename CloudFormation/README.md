# Deploy a High-Availability Web App using CloudFormation

Link showing it successfully works:</br>
http://serve-WebAp-11D6GNCP7035O-557630779.us-west-2.elb.amazonaws.com

## How to

## Login in to your aws console:</br>
1) Go to services
2) Search for CloudFormation click on it
3) Now you can view the stacks you will be creating from the terminal

## Download AWS CLI
Open your Terminal </br>
Download Repository with Code </br>
In terminal type:</br>
`git clone git@github.com:wendysegura/CloudDevOpsEngineer-Program.git`</br>
`cd CloudDevOpsEngineer-Program/CloudFormation/`</br>

Now we can create the stacks from here by running this command:</br>
`./create.sh infrastructure infrastructure.yml infra_parameters.json`</br>
Once that stack has completed you can run:</br>
`./create.sh servers servers.yml server_parameters.json`</br>

You can go to your aws console you should have something like screenshot below </br>


To view your website click on Exports and then click on link next to **DNSName-Link** like screenshot below</br>




