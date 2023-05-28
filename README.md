## php-application-cicd##

CICD of PHP application Using AWS Tools using:
1. EC2 Server
2. AWS Code Build
3. AWS CodePipeline

Scripts folder consist of script to start and stop the httpd service.

Creating an IAM Role for Codedeploy:

a. Go to IAM dashboard through the Services menu.
b. Click on Roles and then Create Role. Select CodeDeploy.
![image](https://github.com/amitks0501/php-application-cicd/assets/76788241/07d6cdfe-5168-4c2e-969c-65be6ac2817e)
c. Click on Next Permissions.  Give it the name "code-deploy-service-role"
![image](https://github.com/amitks0501/php-application-cicd/assets/76788241/c6e7e2eb-a39d-4352-8fc8-a75382ad7c34)


Configuring Codedeploy:

a. Click on Services and Select CodeDeploy.
b. Click on Get Started and Select Custom Deployment option. Skip Walkthrough.




