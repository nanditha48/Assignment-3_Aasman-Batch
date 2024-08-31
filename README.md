# Assignment-3_Aasman-Batch

# Azure Project

## Team Members
1. Nanditha Nambiar [1041750]
2. Shubham Golwal [1041941]
3. Shivani Prasad [1041409]
4. Tanisha Gondke [1041938]

## Overview
This project demonstrates the integration of an Azure Virtual Machine (VM) with Azure Container Instances (ACI) within a Virtual Network (VNet). 

## Project Components
- **Resource Group**: A container that holds related resources for your Azure solution.
- **Virtual Network (VNet)**: A logically isolated network in Azure where both the VM and Container Instances reside.
- **Virtual Machine (VM)**: An on-demand, scalable computing resource in Azure.
- **Azure Container Instances (ACI)**: A service that allows you to run containerized applications in Azure without managing the underlying infrastructure.
- **Networking**: Configuring the VM and Container Instances to communicate securely within the same VNet.

## Prerequisites
- Azure Subscription
- Basic knowledge of Azure Portal and networking concepts
- SSH or RDP client installed on your local machine

## Setup Steps

### 1. Create a Resource Group
1. Sign in to the Azure Portal.
2. In the left-hand menu, select **Resource groups**.
3. Click **+ Add**.
4. Enter a name for the Resource Group.
5. Select your **Subscription** and **Region**.
6. Click **Review + Create**, then **Create**.

### 2. Create a Virtual Network (VNet)
1. Navigate to **Virtual networks** in the Azure Portal.
2. Click **+ Add** to create a new VNet.
3. Provide a name for the VNet and select the same **Subscription** and **Region** as the Resource Group.
4. Configure the **IP Address space** and **Subnets**.
5. Click **Review + Create**, then **Create**.

### 3. Deploy a Virtual Machine (VM)
1. Navigate to **Virtual machines** in the Azure Portal.
2. Click **+ Add** to create a new VM.
3. Select the previously created **Resource Group**.
4. Provide a name for the VM and select the **Region**.
5. Choose an **Image** (e.g., Windows or Linux).
6. Configure the **Size** and **Administrator account**.
7. Under **Networking**, ensure the VM is deployed in the VNet you created earlier.
8. Click **Review + Create**, then **Create**.

### 4. Deploy Azure Container Instances (ACI)
1. Navigate to **Container instances** in the Azure Portal.
2. Click **+ Add** to create a new container instance.
3. Select the same **Resource Group** and **Region** as your VM.
4. Provide a name for the container instance and select an image from Docker Hub or Azure Container Registry.
5. Under **Networking**, choose the VNet and Subnet where your VM resides.
6. Click **Review + Create**, then **Create**.
