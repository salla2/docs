---
title: Creating an AKS Cluster
shortTitle: Azure Kubernetes Service
weight: 2115
aliases:
  - /rancher/v2.x/en/tasks/clusters/creating-a-cluster/create-cluster-azure-container-service/
---

You can use Rancher to create a cluster hosted in Microsoft Azure Kubernetes Service (AKS).

## Prerequisites in the Microsoft Azure Portal 

Obtain the following information from the [Microsoft Azure Portal](https://portal.azure.com) by completing how to [Create Service Principal for Azure AD](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-create-service-principals#create-service-principal-for-azure-ad).

- Your Subscription ID.
- Your Tenant ID.
- A Client ID and Client Secret.

## Create the AKS Cluster

Use Rancher to set up and configure your Kubernetes cluster.

1. From the **Clusters** page, click **Add Cluster**.

2. Choose **Azure Kubernetes Service**.

3. Enter a **Cluster Name**.

4. {{< step_create-cluster_member-roles >}}

5. {{< step_create-cluster_cluster-options >}}

6. Complete the **Account Access** form using the output from your Service Principal. This information is used to authenticate with Azure.

7. Use **Nodes** to provision each node in your cluster and choose a geographical region.

	[Microsoft Documentation: How to create and use an SSH public and private key pair](https://docs.microsoft.com/en-us/azure/virtual-machines/linux/mac-create-ssh-keys)
<br/>
8. Click **Create**.
<br/>
9. Review your options to confirm they're correct. Then click **Create**.

{{< result_create-cluster >}}
