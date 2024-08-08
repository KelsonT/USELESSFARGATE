## Description

#1.  Two files provided.  Template and Role that can be used to deploy the tempate.  
#2.  Optional - Create the role in IAM:Roles using the RoleToDeploy.json 
#3.  Deploy the template via CloudFormation>Stacks>Create stack using options existing template and upload file        *FargateCWtest.yml

        #Provide Stack Name - any string 
        #Provide Params - Select Public Subnet and VPC_ID string
        #If needed add the Role that was created with the RoletoDeply.json under the Permissions
        #Recommended in stack failure options to Preserve successfully provisioned resources 
        #Complete the last checkbox and submit to deploy.  

#4.  A few minuts after the depolyment has completed check in Cloudwatch Logs and you should see a log group called   /aws/fargate/useless-fact-log-group     In the log stream open one of the logs and at the bottom of the log you should see the last two lines show Complete! and the Useless fact. 

