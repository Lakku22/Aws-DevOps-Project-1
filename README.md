# Aws-DevOps-Project-1

The provided steps outline a project for deploying an application using AWS DevOps services. Here's a summary of the key steps:
Step 1: Fetch Code from GitHub

    Clone the application code from GitHub using the command: git clone https://github.com/Aakibgithuber/Aws-DevOps-Project

Step 2: Setup Code Commit

    Create a CodeCommit repository on AWS.
    Create an IAM user with the necessary permissions for CodeCommit.
    Attach the "AWSCodeCommitPowerUser" policy to the IAM user.
    Generate HTTPS Git credentials for CodeCommit.

Step 3: Push Code to Code Commit

    Push the cloned code to the CodeCommit repository using AWS CLI commands.

Step 4: Setup AWS CodeBuild

    Create an AWS CodeBuild project.
    Configure the project with the repository and build specifications.
    Start the build process.

Step 5: Setup S3 Bucket for Code Storage

    Create an S3 bucket for storing the code artifacts.
    Configure CodeBuild to store artifacts in the S3 bucket.

Step 6: Setup Code Deploy

    Create an AWS CodeDeploy application.
    Select EC2 as the deployment target.
    Launch an EC2 instance where the application will be deployed.
    Create IAM roles for EC2 and CodeDeploy with necessary permissions.
    Set up the AWS CodeDeploy agent on the EC2 instance.

Step 7: Create Deployment Group and Deploy Application

    Create a deployment group in AWS CodeDeploy.
    Choose in-place deployment type.
    Select EC2 instances and specify the CodeDeploy agent configuration.
    Deploy the application by providing the S3 path to the code artifacts.

Step 8: Setup Code Pipeline

    Create an AWS CodePipeline to automate the entire process.
    Configure the pipeline with source (CodeCommit), build (CodeBuild), and deploy (CodeDeploy) stages.
    Start the pipeline.

Conclusion

    The deployment is complete, and the application should be accessible on the EC2 instance's public IP.

This project demonstrates a full DevOps workflow, including version control, continuous integration, deployment, and automation using various AWS services.
