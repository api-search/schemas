---
description: Properties of the managed cluster.
layout: schema
name: ManagedClusterProperties
properties_list:
- description: The current provisioning state of the managed cluster resource.
  name: provisioningState
  type: string
- description: The max number of agent pools for the managed cluster.
  name: maxAgentPools
  type: integer
- description: The version of Kubernetes specified by the user. Both patch version (e.g. 1.20.13) and minor version (e.g. 1.20) are supported. When a minor version is specified, the latest supported patch version is
  name: kubernetesVersion
  type: string
- description: The version of Kubernetes the Managed Cluster is running.
  name: currentKubernetesVersion
  type: string
- description: This cannot be updated once the Managed Cluster has been created.
  name: dnsPrefix
  type: string
- description: This cannot be updated once the Managed Cluster has been created. Used only with private clusters with custom private DNS zone.
  name: fqdnSubdomain
  type: string
- description: The FQDN of the master pool.
  name: fqdn
  type: string
- description: The FQDN of private cluster.
  name: privateFQDN
  type: string
- description: The special FQDN used by the Azure Portal to access the Managed Cluster. It is only set for private cluster enabled clusters.
  name: azurePortalFQDN
  type: string
- description: Whether to enable Kubernetes Role-Based Access Control.
  name: enableRBAC
  type: boolean
- description: The support plan for the Managed Cluster.
  name: supportPlan
  type: string
- description: If set to true, getting static credentials will be disabled for this cluster.
  name: disableLocalAccounts
  type: boolean
- description: The name of the resource group containing agent pool nodes.
  name: nodeResourceGroup
  type: string
- description: The agent pool properties.
  name: agentPoolProfiles
  type: array
- description: Identities associated with the cluster.
  name: identityProfile
  type: object
- description: The profile of managed cluster add-ons.
  name: addonProfiles
  type: object
- description: The Resource ID of the disk encryption set to use for enabling encryption at rest.
  name: diskEncryptionSetID
  type: string
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-properties-schema.json
slug: azure-kubernetes-service-managed-cluster-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterProperties\",\n  \"type\": \"object\",\n  \"description\": \"Properties of the managed cluster.\",\n  \"properties\": {\n    \"provisioningState\": {\n      \"type\": \"string\",\n      \"description\": \"The current provisioning state of the managed cluster resource.\"\n    },\n    \"maxAgentPools\": {\n      \"type\": \"integer\",\n      \"description\": \"The max number of agent pools for the managed cluster.\"\n    },\n    \"kubernetesVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of Kubernetes specified by the user. Both patch version (e.g. 1.20.13) and minor version (e.g. 1.20) are supported. When a minor version is specified, the latest supported patch version is chosen automatically.\"\n    },\n    \"currentKubernetesVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of Kubernetes the Managed Cluster is running.\"\
  \n    },\n    \"dnsPrefix\": {\n      \"type\": \"string\",\n      \"description\": \"This cannot be updated once the Managed Cluster has been created.\"\n    },\n    \"fqdnSubdomain\": {\n      \"type\": \"string\",\n      \"description\": \"This cannot be updated once the Managed Cluster has been created. Used only with private clusters with custom private DNS zone.\"\n    },\n    \"fqdn\": {\n      \"type\": \"string\",\n      \"description\": \"The FQDN of the master pool.\"\n    },\n    \"privateFQDN\": {\n      \"type\": \"string\",\n      \"description\": \"The FQDN of private cluster.\"\n    },\n    \"azurePortalFQDN\": {\n      \"type\": \"string\",\n      \"description\": \"The special FQDN used by the Azure Portal to access the Managed Cluster. It is only set for private cluster enabled clusters.\"\n    },\n    \"enableRBAC\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable Kubernetes Role-Based Access Control.\"\n    },\n    \"supportPlan\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The support plan for the Managed Cluster.\"\n    },\n    \"disableLocalAccounts\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to true, getting static credentials will be disabled for this cluster.\"\n    },\n    \"nodeResourceGroup\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the resource group containing agent pool nodes.\"\n    },\n    \"agentPoolProfiles\": {\n      \"type\": \"array\",\n      \"description\": \"The agent pool properties.\"\n    },\n    \"identityProfile\": {\n      \"type\": \"object\",\n      \"description\": \"Identities associated with the cluster.\"\n    },\n    \"addonProfiles\": {\n      \"type\": \"object\",\n      \"description\": \"The profile of managed cluster add-ons.\"\n    },\n    \"diskEncryptionSetID\": {\n      \"type\": \"string\",\n      \"description\": \"The Resource ID of the disk encryption set to use for enabling encryption at rest.\"\n  \
  \  }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-properties-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterProperties
---
