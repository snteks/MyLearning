###1. Why does it take long time to pull image on a fargate pod
    Fargate does not cache images, and therefore the whole image is pulled from the registry when a task runs. The following are our recommendations for images used for Fargate tasks:

    Use a larger task size with additional vCPUs. The larger task size can help reduce the time that is required to extract the image when a task launches.
    Use a smaller base image.
    Have the repository that stores the image in the same Region as the task.

###2. Failed to provision EKS for the first time **Error: "Role with arn: , could not be assumed because it does not exist or the trusted entity is not correct"***
    AWSServiceRoleForAmazonEKS and AWSServiceRoleForAmazonEKSForFargate roles `MUST` be enabled to provision infrastructure via terraform and crossplane

