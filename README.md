# "CLOUD-COMPUTING-CLASS-2020" 
# Lab 4: Creating a web application using cloud PaaS
## Group Members:
- Eudald Sabaté Creixell: eudald.sabate@est.fib.upc.edu
- Julio Candela: julio.christians.candela@est.fib.upc.edu

# Experimentation  

## Task 4.1: Download the repository for the Web App
 
The resources and changes for the web server can be found in the following repository: https://github.com/JulioCandela1993/eb-django-express-signup.git 

## Task 4.2: Create an IAM Policy and Role 

The IAM Policy (gsg-signup-policy) and Role (gsg-signup-role) were succesfully created 

## Task 4.3: Create a DynamoDB Table 

The gsg-signup-table was sucessfully created in Ireland region.

![Test Local Server 4.4.1](Images/4.3_DynamoTable.PNG)

## Task 4.4: Test the web app locally

Before the execution, we had to modify the file environment.bat (Windows) since we got some problems in the set of variables (without quotes) and be sure that the aws configuration was set to the region specified (eu-west-1, you can use the command "aws configure"):

##### @ECHO OFF 
##### SET DEBUG="True" 
##### SET STARTUP_SIGNUP_TABLE=gsg-signup-table 
##### SET AWS_REGION=eu-west-1
##### ECHO %DEBUG%, %STARTUP_SIGNUP_TABLE%, %AWS_REGION%

The server is succesfully running after executing the python scripts:

![Test Local Server 4.4.1](Images/4.4_1_LocalServer.PNG)

In order to validate the result of the insertion, we opened the DynamoDB console in AWS and get the elements stored in the table (our email accounts, names and decisions of preview)

![Test Local Server 4.4.2](Images/4.4_2_LocalTest.PNG)

## Task 4.5: Create the AWS Beanstalk environment and deploy the sample web app

## Task 4.6: Configure Elastic Beanstalk CLI and deploy the target web app

## Questions

### Q45b: What has happened? Why do you think that has happened?

### Q45c: Can you terminate the application using the command line? What is the command? if it exists.

### Q45d: What parameters have you added to the eb create command to create your environment? Explain why you have selected each parameter.

### Q46: How long have you been working on this session? What have been the main difficulties you have faced and how have you solved them? 