# 2048-Game-Deployment-on-AWS-EKS
2048 Game Deployment on AWS EKS

This project focuses on deploying a game onto a Kubernetes cluster, utilizing AWS Elastic Kubernetes Service. 
The deployed 2048-Game is depicted in the picture below.

AWS Services Used: AWS EKS, AWS Fargate, Application Load Balancer, IAM, AWS CLI, AWS VPC.

🛠️ Steps involved:
1. Set up prerequisites: awscli, eksctl, and kubectl.
2. Installed EKS with Fargate.
3. Acquired or updated the KubeConfig file for CLI access to cluster resources.
4. Created a "game-2048" namespace linked to the Fargate profile "alb-sample-app."
5. Deployed the 2048 app as a K8s Pod, created a corresponding service, and set up an Ingress resource for traffic routing.
6. Implemented the Ingress Controller to automate ALB Controller creation.
7. Established an IAM OIDC Provider to grant ALB Controller access to the Application Load Balancer.
8. Created a service account with an IAM Role and Policy for Load Balancer access.
9. Deployed ALB Controller using Helm Charts, interfacing with the service account.
10. Accessed the deployed 2048 application in EKS.


![Deployed App](https://github.com/abrarpasha24/2048-Game-Deployment-on-AWS-EKS/assets/30976576/f9ac35d2-4aca-4b7c-82d2-57b31d98a46d)
