# k8s-apps
Sample k8s apps

## Description

This repository constains some yaml files with kubernetes deployments and services definitions to enable a useful example how to apply a GitOps methods into kubernetes applications and cluster. 

If you are curious about what is a GitOps model, please check the [Guide to GitOps](https://www.weave.works/technologies/gitops/) from Weaveworks

We have setup a GitHub Actions Workflow to properly connect and manage kubernetes deployments, services definitions and etc.

## Prerequisites and recommendations
1. A public Kubernetes API endpoint so GitHub can reach your cluster
2. Create an IAM user with sufficient access to connect into AWS cluster and list EKS resorces
3. Export the `ACCESS_KEY` and `SECRET_KEY` and save into the repository Secrets
4. Configure and customize the GitHub workflow to act upon your desired branches.

## Usage
The workflow is configured to apply a `kubectl apply -f app/nginx.yaml` into the cluster for every new push into the main branch.

## License
MIT

