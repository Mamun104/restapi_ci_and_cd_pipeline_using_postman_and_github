# Rest API CI And CD Pipeline Using Postman And Github

## Technology and Tool Used
- Postman
- Visual Studio Code
- CI AND CD
- Github
- Terminal

## Prerequisites

- You must have installed Postman to your system
- Install Postman CLI

## Scenario of this project

- The user can create a user
- The user can create a user by id,name
- The user can get all users
- The user can get individual user by user id
- The user can update a user by user id
- The user can delete a user by user id

## API Documents

  https://documenter.getpostman.com/view/16548351/2s9Y5SWRC4

## ## How to set up Postman CLI

### Step-1:

- Open the Postman
- Create a workspace
- Create a collection

### Step-2:
- Click the collection
  
  ![image](https://github.com/Mamun104/restapi_automation_run_on_postman_cli/assets/78067017/5ae3cde3-e3f8-492b-8ad8-58fb800a7fd9)

- then click the collection run button

  ![image](https://github.com/Mamun104/restapi_automation_run_on_postman_cli/assets/78067017/6ee1dab5-47e6-4fb8-87f5-d314543fa1fc)
- then click the automate run via cli

  ![image](https://github.com/Mamun104/restapi_automation_run_on_postman_cli/assets/78067017/2197efd6-e3ad-4022-ab71-02a7bb470b7c)
### Step-3

- then install postman cli from here

               https://learning.postman.com/docs/postman-cli/postman-cli-installation/#windows-installation
- open the terminal
- hit the commmand
- after postman cli install then generate a api key
- then login with this command in cmd

              postman login --with-api-key {{xyz}}
  
- after login successfully then hit this command in cmd

             postman collection run {{collection_key}}
  ![image](https://github.com/Mamun104/restapi_automation_run_on_postman_cli/assets/78067017/b05fae3a-3b00-48bb-b75c-4c59ed3de8b1)

### Step-4

- Click the run on ci and cd

![image](https://github.com/Mamun104/restapi_ci_and_cd_pipeline_using_postman_and_github/assets/78067017/25582ac2-10a9-485b-a420-d158096a388f)

- then Generate Postman CLI Configuration

![image](https://github.com/Mamun104/restapi_ci_and_cd_pipeline_using_postman_and_github/assets/78067017/ee098a91-d6cc-4d72-ba65-bc3c50a64682)

- after that copy postman cli command

![image](https://github.com/Mamun104/restapi_ci_and_cd_pipeline_using_postman_and_github/assets/78067017/f9191c0b-3f68-4fb5-8dd4-3ff308744f99)

### Step-5

- create a new repository via github
- then click the github action

![image](https://github.com/Mamun104/restapi_ci_and_cd_pipeline_using_postman_and_github/assets/78067017/eb449f88-7fab-47b7-80ce-27e0526ef8da)

- then select the simple workflow

![image](https://github.com/Mamun104/restapi_ci_and_cd_pipeline_using_postman_and_github/assets/78067017/51da6529-8e50-4b1f-ae37-c21fc2fb7846)

- then copy and paste the postman cli command
- after that can commit this file
- then click the github action and run this file


## What is CI:
Continuous delivery (CD) is the automated delivery of completed code to environments like testing and development. CD provides an automated and consistent way for code to be delivered to these environments.

## What is CD:
Continuous deployment is the next step of continuous delivery. Every change that passes the automated tests is automatically placed in production, resulting in many production deployments.

Continuous deployment should be the goal of most companies that are not constrained by regulatory or other requirements.

![image](https://github.com/Mamun104/restapi_ci_and_cd_pipeline_using_postman_and_github/assets/78067017/cc3dc2ae-ec10-46eb-9b2c-312e1cf68c1d)


## How to work ci and cd pipeline

Working with a CI/CD pipeline involves several key steps, from code development to deployment. Here's a simplified overview of how you can work with a CI/CD pipeline:

### Develop Code:
Start by writing your code or making changes to existing code. Ensure you follow best practices for version control (e.g., Git) and create feature branches for your work.

### Commit Code:
After completing a piece of work, commit your changes to the version control system. Make sure your commits are descriptive and include relevant comments.

### Automated Build:
Once you push your changes to the repository, the CI/CD pipeline should automatically trigger a build process. During the build, the pipeline compiles your code, packages it into deployable artifacts, and prepares it for testing.

### Automated Testing:
The CI/CD pipeline should execute automated tests as part of the process. These tests can include unit tests, integration tests, and any other test suites relevant to your project. If any tests fail, the pipeline may halt, and you'll be notified of the issue.

### Deployment (Optional):
If your pipeline includes deployment stages, it will deploy the code to a staging or production environment automatically. This typically involves deploying to a test environment first to ensure everything works as expected before deploying to production.

### Monitoring and Notifications:
During and after deployment, the CI/CD pipeline should provide you with monitoring data and notifications. You can track the progress of your build and deployment, check for errors or performance issues, and receive alerts if anything goes wrong.

### Manual Approval (Optional):
In some cases, you may want to include manual approval steps before deploying to production. This allows a team member to review and approve the changes before they go live.

### Rollback (Optional):
If an issue is detected in the production environment, the CI/CD pipeline should have a rollback mechanism in place to revert to the previous stable version of the application.

### Post-Deployment Tasks:
After deployment, you may need to perform post-deployment tasks, such as database migrations, cache clearing, or other environment-specific actions.

### Logging and Metrics:
Make use of logging and metrics to gather information about the application's behavior in production. This data can help you troubleshoot issues and improve performance.

### Continuous Improvement:
Regularly review the CI/CD pipeline and its configuration to identify areas for improvement. This could include optimizing build times, enhancing test coverage, or streamlining deployment processes.

### Documentation and Collaboration:
Ensure that your team understands how the CI/CD pipeline works and how to use it effectively. Document the pipeline's setup and workflows to facilitate collaboration.

### Security and Compliance:
Implement security checks and compliance measures as part of your pipeline to ensure code quality and security.

### Scaling:
As your project grows, you might need to scale your CI/CD pipeline to handle increased workloads and more complex deployments.

### Maintenance:
Regularly update and maintain your CI/CD tool, dependencies, and scripts to ensure ongoing reliability and security.

Remember that the specific steps and tools you use in your CI/CD pipeline can vary based on your project's requirements and technology stack. The key is to automate as much of the development, testing, and deployment processes as possible to ensure a consistent and reliable workflow.


## what is postman cli

Postman CLI (Command Line Interface) is a tool that allows you to run Postman collections and environments from the command line, making it easy to automate and integrate API testing and monitoring into your development and CI/CD pipelines
