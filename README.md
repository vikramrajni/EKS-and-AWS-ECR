**AWS EKS CI/CD Pipeline for Java Application**

Designed and implemented a complete CI/CD pipeline to build, package, containerize, and deploy a Java application to an AWS EKS Kubernetes cluster using Jenkins, Maven, Docker, and AWS ECR.

**Key Components**
 - Created an Amazon ECR (Elastic Container Registry) repository to store Docker images.
 - Configured AWS credentials in Jenkins to enable secure authentication and image pushes to ECR.
 - Created a Kubernetes imagePullSecret in AWS EKS, allowing the cluster to securely pull container images from ECR.
 - Developed a Jenkins CI/CD pipeline to automate the application delivery process.

**Jenkins Pipeline Functionality**
 - Automatically increments the application version.
 - Builds and packages the Java application using Maven.
 - Creates a Docker image containing the application.
 - Pushes the Docker image to AWS ECR.
 - Deploys the updated image to AWS EKS.
 - Updates the application version in pom.xml.
 - Commits and pushes version changes back to the Git repository.
