# 🚀 CI/CD for Dockerized 2048 Game

Automated build and deployment pipeline for the 2048 game

## Short Description

Implemented a full end-to-end CI/CD pipeline that containerizes the 2048 game with Docker, automates build/test, pushes images to a registry, and deploys to AWS using managed services—ensuring rapid, reliable delivery.

## 🛠️ AWS Services Used:

Amazon ECR,
AWS CodeBuild,
Amazon ECS (or AWS Fargate),
AWS CodePipeline,
AWS IAM,

## 🧰 Technical Tools:

Docker,
GitHub Actions (or AWS CodePipeline),
YAML Pipeline Definitions,
Bash/Shell scripting,

## 🧠 Skills Demonstrated:

Containerization best practices,
CI/CD pipeline orchestration,
Infrastructure as Code & cloud deployments,
Automated testing and quality gates,

## 📋 Steps Performed

### Clone and Containerize the Game:

Cloned the 2048 game repository.
Built a multi-stage Dockerfile to produce a lean runtime image.

### Push Image to Container Registry:

Created an ECR repository.
Configured CI step to authenticate, tag, and push the Docker image.

### Define CI Pipeline:

Set up CodeBuild (or GitHub Actions) to run linting, unit tests, image build/push.
Configured CodePipeline stages: source → build → deploy.

### Provision and Deploy to ECS/Fargate:

Defined ECS cluster and service (or Fargate task).
Configured deploy step to pull the latest image and update the service with zero-downtime.

### Monitor and Validate Deployment:

Enabled CloudWatch logs and metrics for the service.
Validated application endpoint and ensured new image versions reflected changes automatically.

## ✅ Final Result:

Fully automated CI/CD pipeline for Dockerized 2048 game

## 💼 Business Implication:

This project illustrates how to establish a cloud-native CI/CD workflow for containerized applications, enabling faster feature delivery, higher reliability, and consistent builds. It empowers DevOps teams to deploy changes with confidence while reducing manual overhead and operational risk.
