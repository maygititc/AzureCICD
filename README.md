"# AzureCICD" 


Provision Infrastructure with Terraform:

Installs Terraform.

Initializes and validates the Terraform configuration.

Applies the Terraform plan to provision infrastructure (e.g., AKS cluster, ACR).

Build and Publish Docker Image to ACR:

Builds a Docker image from the application's Dockerfile.

Pushes the Docker image to Azure Container Registry (ACR) with a unique tag.

Deploy to Kubernetes using Helm:

Installs Helm.

Retrieves AKS credentials to authenticate with the Kubernetes cluster.

Deploys the application to AKS using a Helm chart, specifying the image repository and tag.

Prerequisites
Terraform Configuration:

Ensure you have a infrastructure directory with Terraform files (main.tf, variables.tf, etc.) to provision the required infrastructure.

Dockerfile:

Ensure your application has a Dockerfile for building the Docker image.

Helm Chart:

Ensure you have a Helm chart in a helm directory (e.g., helm/my-app-chart) with a values.yaml file and templates.

Azure DevOps Service Connection:

Set up an Azure service connection in Azure DevOps to authenticate with your Azure subscription.

ACR and AKS:

Ensure the ACR and AKS cluster are provisioned (either manually or via Terraform).