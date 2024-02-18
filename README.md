# Image Upgrade in Azure

This repository provides step-by-step instructions for upgrading images in Azure using Packer, GitHub Actions, and Azure Virtual Machine Scale Sets (VMSS). The process involves creating a self-hosted runner, cloning the repository, building an image with Packer, and automatically updating the image in the VMSS.

## Instructions

### 1. Create a Self-Hosted Runner
Before getting started, create a self-hosted runner in your Virtual machine. This runner will be used to execute the workflows in this repository.

### 2. Clone the Repository
Clone this repository to your local environment and cd to the repo and trigger the workflow:


## Flow Diagram

The bellow diagram illustrates the flow of the image upgrade process.



![Screenshot from 2024-02-09 14-32-15](https://github.com/OsandaDhananjaya/PackerImageBuild/assets/101936340/7a430efc-e728-4f22-94c1-26309876ecdf)

### Github action workflow

### 1) Pipeline Activation:
Trigger the continuous integration pipeline to commence the build process.

### 2) Packer Image Building:

Execute the Packer build command to create a customized image, ensuring adherence to security and configuration standards.

### 3) Azure Image Deployment:

Deploy the newly created image to the Azure Images, maintaining versioning and tagging conventions for traceability.

### 4) Scale Set Image Update:

Utilize Azure CLI commands to seamlessly update the image associated with the targeted Azure Virtual Machine Scale Set.

