
Pre-Requisite:
The Codedeploy configurations are completed, then only proceed with the pipeline creation.

1. Search Codepipeline and select "Create Pipeline"
2. Enter the name of the pipeline you want to create and select New service role and click Next.

![image](https://github.com/amitks0501/php-application-cicd/assets/76788241/ac7bec70-d0f6-461d-8eda-e770eadb5c88)

3. Source Provider : This option describes the CI part ie where our code is maintained. Upon a successfull push by developer to the code repository the pipeline will
   get triggered. The source provider is the service which you use to store your code. ie GitHub, AWS Code commit. We are using AWS Code commit to store the code, select 
   github, if you are using github.
    
![image](https://github.com/amitks0501/php-application-cicd/assets/76788241/b548b1b8-845d-4b19-98eb-6d45904ffecd)

4. Click on the Skip build page.

![image](https://github.com/amitks0501/php-application-cicd/assets/76788241/e24af1af-fe09-4cc8-9973-e8999a024427)

5. Select AWS Code Deploy, Select the region where the Code Deploy was created; the Application name and the Deployment group created earlier.

![image](https://github.com/amitks0501/php-application-cicd/assets/76788241/a471586e-03e8-4a8d-acd8-cdcef4f1221e)

6. Review  the settings and click on create pipeline.

7. To test the Pipeline, commit and push changes to the code repository and view the pipeline status. It will be deployed successfully.


