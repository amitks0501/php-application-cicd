## php-application-cicd##

CICD of PHP application Using AWS Tools using:
1. EC2 Server
2. AWS Code Build
3. AWS CodePipeline

Pre-Requisite:
a. An EC2 instance with LAMO stack installed. Please check the following guide: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-lamp-amazon-linux-2.html

b. Code deploy agent installed on the instance. https://docs.aws.amazon.com/codedeploy/latest/userguide/codedeploy-agent-operations-install-linux.htm



Scripts folder hold the command to start and stop the httpd service.


Creating an IAM Role for Codedeploy:

a. Go to IAM dashboard through the Services menu.

b. Click on Roles and then Create Role. Select CodeDeploy.
![image](https://github.com/amitks0501/php-application-cicd/assets/76788241/07d6cdfe-5168-4c2e-969c-65be6ac2817e)

c. Click on Next Permissions.  Give it the name "code-deploy-service-role"
![image](https://github.com/amitks0501/php-application-cicd/assets/76788241/c6e7e2eb-a39d-4352-8fc8-a75382ad7c34)


Configuring Codedeploy:

a. Click on Services and Select CodeDeploy.
b. Click on Getting Started and Select > Create Application

![image](https://github.com/amitks0501/php-application-cicd/assets/76788241/885a4d58-f761-4112-88a7-484574aa0b08)
c. Input a suitable name for your application and then click Create Application.
![image](https://github.com/amitks0501/php-application-cicd/assets/76788241/9688f212-1073-438d-91e2-2aa3693272bd)

d. Click on create deployment group.
![image](https://github.com/amitks0501/php-application-cicd/assets/76788241/fc3e4a71-eb3b-446c-b7ac-7b23f1736a44)

e. Enter a relevant name as per your requirement. Select the Code deploy role you had create earlier and choose In-place option since we only have single instance.
![image](https://github.com/amitks0501/php-application-cicd/assets/76788241/85edd910-9cb3-4a03-81c9-639c1a3252fd)

f. In the environment configuration we need to choose on which instance the application will be deployed. As part of pre requisite we had created a instance with LAMP configuration installed and Codedeploy agent installed.. Enter the name of the server.

![image](https://github.com/amitks0501/php-application-cicd/assets/76788241/ecd91733-70c4-47f5-8f31-35b3c5718e23)

g. Click never for the option to install codedeploy agent (since we have already installed it). Uncheck the "Enable load balancing".

![image](https://github.com/amitks0501/php-application-cicd/assets/76788241/9f72f465-222f-4b03-950b-af2e322ff054)





