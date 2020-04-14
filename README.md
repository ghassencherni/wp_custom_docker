# wp_custom_docker
Pipeline (Jenkinsfile) to Build and push customized images ( ghassen-devopstt) on Guitlab Registry, it comes with other projects : [deploy_jenkins](https://github.com/ghassencherni/deploy_jenkins), [terraform_aws_eks](https://github.com/ghassencherni/terraform_aws_eks) and [wordpress_k8s](https://github.com/ghassencherni/wordpress_k8s).

Please start loocking in [deploy_jenkins](https://github.com/ghassencherni/deploy_jenkins) First.

## Getting Started

This Jenkins file allows to build images based on wordpress-4.8-apache ( Dockerfile ) then push them to Gitlab Registry and trigger [wordpress_k8s](https://github.com/ghassencherni/wordpress_k8s) pipeline in order to deploy the new image on EKS

## Requirements

- Gitlab account ( user and password ) must be stored on Jenkins ( Global credential ) with the id "gitlab_registry"

