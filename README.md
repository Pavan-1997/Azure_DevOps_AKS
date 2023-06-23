# Azure DevOps deploying application on AKS Cluster

In this project I have setup a Azure pipeline where the source code is fetched from my GitHub, Pipeline was setup having tasks for Maven, Push Artifact, Push Image to ACR 

I have created a release pipeline to deploy my application on Azure AKS cluster using the manifest file present in my repo.

The pipeline is executed on agent where I have made use of a EC2 Ubuntu machine to run the jobs.

At the end the application is accessed by the Load Balancer IP created by Kubernetes on Azure.

All the commands are documented in the CMD.txt file

Below is the image of my release pipeline:

![release](https://github.com/Pavan-1997/Azure_DevOps_AKS/assets/32020205/daa3d0b8-49e7-45f5-a984-a0d6af17fc22)


Below are the images of my shopping cart application:

![app-2](https://github.com/Pavan-1997/Azure_DevOps_AKS/assets/32020205/ff12069e-6724-45b9-a09a-453e37a3ad19)

![app-1](https://github.com/Pavan-1997/Azure_DevOps_AKS/assets/32020205/bd403ee8-9149-40ec-8fa3-d10690564fcf)

![app](https://github.com/Pavan-1997/Azure_DevOps_AKS/assets/32020205/8945803f-858e-4d11-987c-69f2a562f850)
