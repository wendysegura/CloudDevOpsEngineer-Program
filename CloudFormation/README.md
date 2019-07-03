#Deploy a High-Availability Web App using CloudFormation

##Parameters: More than 1 </break>
##Resources: LoadBalancer, Launch Configuration, AutoScaling group a health check, security groups and Listner and Target Group</break>
##Outputs: URL with Load Balancer DNS Name and "http" in front of it</break>
##Working Test: Url to verify it works with page that reads "it works! Udagram, Udacity"</break>

#Load Balancer</break>
#Target Group: The auto-scaling group needs to have a property that associates it with a target group. The Load Balancer will have a Listener rule associated with the same target group.</break>
#Health Check and Listener: Port 80 should be used in Security groups, health checks and listeners associated with the load balancer</break>

#Auto-Scaling</break>
#Subnets: Students should be using PRIV-NET ( private subnets ) for their auto-scaling instances.</break>
#Machine Specs: The machine should have 10 GB or more of disk and should be a t3.small or better.</break>
#SSH Key: There shouldn’t be a ‘keyname’ property in the launch config.</break>
