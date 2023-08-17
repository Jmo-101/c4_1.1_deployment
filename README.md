<p align="center">
<img src="https://github.com/kura-labs-org/kuralabs_deployment_1/blob/main/Kuralogo.png">
</p>
<h1 align="center">C4_deployment-1.1<h1> 

# Workflow Documentation

## 1. GitHub

- Downloaded files from GitHub repository
- Uploaded files into a new GitHub repository

## 2. Jenkins

- Logged into Jenkins and created a new pipeline
- Created a new pipeline using a new repository
- Had to generate a new GitHub repository token to use as credentials on Jenkins
- Saved credentials and ran the pipeline. Success

## 3. Elastic Beanstalk

- Created Elastic Beanstalk permissions
- Created IAM permissions
- Went into Elastic Beanstalk to create an application based on the GitHub repository
- Made sure to upload the GitHub repository to the Beanstalk application
- Added an availability zone to the application

## 4. Troubleshooting

- Ran into a problem on Elastic Beanstalk
- Downloaded logs from Beanstalk to troubleshoot
- While reading the logs, noticed it said error "ModuleNotFound:application"
- Upon further inspection, noticed the module that was not found was located in GitHub.
- The name of the file was incorrect.
- Renamed the file from "app" to "application" and successfully deployed the application
