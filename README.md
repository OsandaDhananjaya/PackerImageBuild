# Image Upgrade in Azure

This repository provides step-by-step instructions for upgrading images in Azure using Packer, GitHub Actions, and Azure Virtual Machine Scale Sets (VMSS). The process involves creating a self-hosted runner, cloning the repository, building an image with Packer, and automatically updating the image in the VMSS.

## Instructions

### 1. Create a Self-Hosted Runner
Before getting started, create a self-hosted runner in your Virtual machine. This runner will be used to execute the workflows in this repository.

### 2. Clone the Repository
Clone this repository to your local environment using the following command and cd to the repo and trigger the workflow:

bash
```git clone``` ~ https://github.com/your-username/your-repo.git~


```cd your-repo```

## Flow Diagram

The bellow diagram illustrates the flow of the image upgrade process.



![Screenshot from 2024-02-09 14-32-15](https://github.com/OsandaDhananjaya/PackerImageBuild/assets/101936340/7a430efc-e728-4f22-94c1-26309876ecdf)




