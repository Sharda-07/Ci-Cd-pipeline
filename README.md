# Ci-Cd-pipeline

Project Report : CI/CD Pipeline on AWS

Project Overview:- This project demonstrates the implementation of a Continuous Integration/Continuous Deployment (CI/CD) pipeline using Jenkins. The pipeline is triggered by a webhook and deployed on an Amazon EC2 machine. The setup ensures seamless integration, testing, and deployment of code changes.

Objectives:- To automate the build, test, and deployment processes. To ensure rapid and reliable integration of code changes. To minimise manual intervention and reduce the chances of errors during deployment.

Components Used:- Jenkins: An open-source automation server used to build, test, and deploy software. 
Webhook: A method used to trigger the Jenkins pipeline automatically upon code changes. 
Amazon EC2: A scalable virtual server in the cloud where the application is deployed. 
Version Control System (e.g., GitHub): To manage source code and track changes.

Project Setup:- Setting Up Jenkins on EC2 Launched an Amazon EC2 instance with appropriate security groups and configurations. Installed Jenkins on the EC2 instance. Configured Jenkins to run as a service for continuous availability. Configuring Jenkins Installed necessary plugins such as Git, Pipeline, and SSH Agent. Set up credentials for accessing the Git repository and the EC2 instance. Creating a Jenkins Pipeline Defined a Jenkins Pipeline using a Jenkinsfile which includes stages for: 
Checkout: Cloning the repository from Git. 
Build: Compiling the code. 
Test: Running automated tests. 
Deploy: Deploying the application to the EC2 instance. Setting Up Webhook Configured a webhook in the version control system (e.g., GitHub) to notify Jenkins of any code changes. The webhook triggers the Jenkins pipeline automatically upon every push to the repository. Deployment on EC2 Utilized SSH and SCP within the Jenkins pipeline to deploy the built application to the EC2 instance. Verified the deployment by checking the application’s status on the EC2 instance.

Pipeline Workflow Code Commit:- Developers commit changes to the Git repository. 
Webhook Trigger:- The webhook triggers the Jenkins pipeline. 
Pipeline Execution:- Checkout: The pipeline checks out the latest code from the repository. 
Build:- The code is built. 
Test:- Automated tests are executed to ensure code quality. 
Deploy:- The successful build is deployed to the EC2 instance. 
Notification:- Notifications are sent to the team upon successful deployment or in case of any failure.

Benefits:- 
Automation: Reduces manual intervention, speeding up the release process. 
Consistency: Ensures that every deployment follows the same process. 
Scalability: Easily scalable to accommodate more complex workflows and additional environments. 
Feedback: Provides immediate feedback to developers through automated testing and notifications.

Conclusion:- This project successfully demonstrates the power and flexibility of Jenkins in automating the CI/CD pipeline, leveraging webhooks for seamless integration, and deploying applications on Amazon EC2. The setup enhances productivity, ensures higher code quality, and accelerates the deployment process.
