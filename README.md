# Azure DevOps deploying application on AKS

In this project I have setup an Azure pipeline where the source code is fetched from my GitHub, Pipeline was setup have tasks for Maven, Push Artifact, and Push Image to ACR.

I have created a release pipeline where the shopping cart application is deployed on the AKS cluster using the manifest file in my repo.

The pipeline is executed on an agent where I have made use of an EC2 Ubuntu machine to run the jobs.

Service connections are created when required during the project.

At the end the application is accessed using the Load Balancer IP which is created by Kubernetes on Azure

All the commands are documented in the CMD.txt file

Below is an image of the release pipeline tasks:

![release](https://github.com/Pavan-1997/Azure_DevOps_AKS/assets/32020205/773f895f-a58a-416e-a682-7e8c48148072)

Below is an image for the pods created as part of the replica set:

![pods](https://github.com/Pavan-1997/Azure_DevOps_AKS/assets/32020205/f16d5efd-91dc-472f-b88d-7d4fe32bba5e)

Below is an image for the services and load balancer created as part of the deployment:

![services](https://github.com/Pavan-1997/Azure_DevOps_AKS/assets/32020205/cb1878b7-7bb8-4999-80ad-bd93d225d7ca)
