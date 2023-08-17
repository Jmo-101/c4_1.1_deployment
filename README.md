<p align="center">
<img src="https://github.com/kura-labs-org/kuralabs_deployment_1/blob/main/Kuralogo.png">
</p>
<h1 align="center">C4_deployment-1.1<h1> 

# Workflow Documentation

# About

Welcome to this repository. This repository is a Jenkins and Elastic Beanstalk project where we took this file code and ran it through Jenkins to ensure everything was correct and then deployed it through AWS Elastic Beanstalk. Along the way, there were a few errors that had to be corrected. Below are the steps I took to achieve the success of the deployment.


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

## Conclusion

Through a combination of Jenkins automation and AWS Elastic Beanstalk deployment, we successfully deployed the code from this repository



<img width="500" alt="Screenshot 2023-08-16 at 12 31 45 PM" src="https://github.com/Jmo-101/c4_1.1_deployment/assets/138607757/a0fe2c95-7330-4613-9656-eb750bfde3e7">
  
  <img width="500" alt="Screenshot 2023-08-16 at 8 59 21 PM" src="https://github.com/Jmo-101/c4_first_deployment/assets/138607757/2b90bae0-88d0-44f6-9893-bcf3bf41a0c1">


<img width="500" alt="Screenshot 2023-08-16 at 8 44 55 PM" src="https://github.com/Jmo-101/c4_1.1_deployment/assets/138607757/5e9fced3-18db-4e76-8d10-73f410754e55">
