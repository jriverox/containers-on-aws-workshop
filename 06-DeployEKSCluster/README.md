## Deploying a Kubernetes Cluster using EKS

## Elastic Container Service for Kubernetes (EKS)

[Elastic Kubernetes Service](https://aws.amazon.com/eks/getting-started) is AWS-managed Kubernetes cluster orchestration service. With EKS you will be able to launch highly-available Kubernetes clusters without spending time on undifferentiated heavy-lifting regarding managing the underlying infrastructure.

![EKS How It Works](images/eks-how-it-works.png)

**Quick jump:**

* [1. Tutorial Overview](/08-DeployEKSCluster#1-tutorial-overview)
* [2. Creating the Cluster](/08-DeployEKSCluster#2-creating-the-cluster)
* [3. Creating the ALB](/08-DeployEKSCluster#3-creating-the-alb)
* [4. Creating the Task Definition](/08-DeployEKSCluster#4-creating-the-task-definition)
* [5. Creating the Service](/08-DeployEKSCluster#5-creating-the-service)
* [6. Testing our service deployments from the console and the ALB](/08-DeployEKSCluster#6-testing-our-service-deployments-from-the-console-and-the-alb)
* [7. That's a wrap!](/08-DeployEKSCluster#7-thats-a-wrap)

## 1. Tutorial Overview

During this hands-on labs we'll walkthrough creating an EKS Cluster and deploy our early created containers on it. It's important to had completed [00-Application](../00-Application/), [01-SetupEnvironment](../01-SetupEnvironment/), [02-CreatingDockerImage](02-CreatingDockerImage/) and [03-CreateVPC](../03-CreateVPC/). Having being able to successfully complete [04-DeployEcsCluster](04-DeployEcsCluster/) lab would be very helpful here too.

## 2. Creating the Cluster

Once logged into [AWS Management Console](https://console.aws.amazon.com/console/home), open [EKS Console](https://console.aws.amazon.com/eks/home), which is currently available on `us-east-1`, `us-west-2` and `eu-west-1`.

If it's your first time on EKS Console you'll see the following:

![EKS Console](images/eks-home.png)

