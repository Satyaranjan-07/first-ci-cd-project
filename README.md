CI/CD PIPELINE FOR NODE.JS APPLICATION
Project Overview:
This project demonstrates a basic CI/CD pipeline built using GitHub Actions and Docker. The goal of this project is to understand how code changes can be automatically built and packaged using a CI/CD workflow.
Whenever code is pushed to the main branch, the pipeline runs automatically to install dependencies, build a Docker image, and push it to DockerHub.
This project was developed as part of my learning journey in DevOps and cloud fundamentals.

TECHNOLOGIES USED:
Git and GitHub
GitHub Actions
Node.js (v18)
Docker
DockerHub
Linux (Ubuntu)

CI/CD WORKFLOW DESCRIPTION:
The CI/CD workflow is defined in the following file:
.github/workflows/main.yml

WORKFLOW STEPS:
1 - The pipeline is triggered on every push to the main branch.
2 - The source code is checked out from the GitHub repository.
3 - Node.js version 18 is set up on the GitHub Actions runner.
4 - Project dependencies are installed using npm install.
5 - A test stage is included as a placeholder for future test automation.
6 - The pipeline securely logs in to DockerHub using GitHub Secrets.
7 -A Docker image is built using the Dockerfile.
8 -The built image is pushed to DockerHub automatically.

GITHUB SECRETS CONFIGURATION:
To ensure security, DockerHub credentials are stored using GitHub Secrets:
1 - DOCKER_USERNAME
2 - DOCKER_PASSWORD
3 -3DOCKER_REPO
These secrets are accessed during the workflow to authenticate and push the Docker image.

DOCKER INTEGRATION:
The project includes a Dockerfile that packages the Node.js application into a container. This helps maintain consistency across different environments and supports automated deployment.

WHAT I LEARNED:

1 - Basics of CI/CD pipelines
2 - Automating workflows using GitHub Actions
3 - Secure credential management with GitHub Secrets
4 -Building and pushing Docker images
5 - Understanding DevOps workflow fundamentals

CI/CD pipeline worked successfully.
