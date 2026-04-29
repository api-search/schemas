---
description: Properties of a managed cluster.
layout: schema
name: ManagedClusterProperties
properties_list:
- description: The current provisioning state.
  name: provisioningState
  type: string
- description: ''
  name: powerState
  type: object
- description: The version of Kubernetes specified by the user.
  name: kubernetesVersion
  type: string
- description: The current version of Kubernetes running on the cluster.
  name: currentKubernetesVersion
  type: string
- description: This cannot be updated once the managed cluster has been created.
  name: dnsPrefix
  type: string
- description: The FQDN of the master pool.
  name: fqdn
  type: string
- description: The FQDN subdomain.
  name: fqdnSubdomain
  type: string
- description: The agent pool properties.
  name: agentPoolProfiles
  type: array
- description: The profile for Linux VMs.
  name: linuxProfile
  type: object
- description: The profile for Windows VMs.
  name: windowsProfile
  type: object
- description: Information about the service principal identity for the cluster.
  name: servicePrincipalProfile
  type: object
- description: The profile of managed cluster add-on.
  name: addonProfiles
  type: object
- description: The name of the resource group containing agent pool nodes.
  name: nodeResourceGroup
  type: string
- description: Whether to enable Kubernetes RBAC.
  name: enableRBAC
  type: boolean
- description: Whether to enable Kubernetes pod security policy (deprecated).
  name: enablePodSecurityPolicy
  type: boolean
- description: Parameters to be applied to the cluster autoscaler.
  name: autoScalerProfile
  type: object
- description: Access profile for managed cluster API server.
  name: apiServerAccessProfile
  type: object
- description: The resource ID of the disk encryption set.
  name: diskEncryptionSetID
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-kubernetes-service-managed-cluster-properties-schema.json
slug: azure-kubernetes-service-managed-cluster-properties
source_filename: azure-kubernetes-service-managed-cluster-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterProperties\",\n  \"type\": \"object\",\n  \"description\": \"Properties of a managed cluster.\",\n  \"properties\": {\n    \"provisioningState\": {\n      \"type\": \"string\",\n      \"description\": \"The current provisioning state.\"\n    },\n    \"powerState\": {\n      \"type\": \"object\"\n    },\n    \"kubernetesVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of Kubernetes specified by the user.\"\n    },\n    \"currentKubernetesVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The current version of Kubernetes running on the cluster.\"\n    },\n    \"dnsPrefix\": {\n      \"type\": \"string\",\n      \"description\": \"This cannot be updated once the managed cluster has been created.\"\n    },\n    \"fqdn\": {\n      \"type\": \"string\",\n      \"description\": \"The FQDN of the master pool.\"\n    },\n    \"fqdnSubdomain\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The FQDN subdomain.\"\n    },\n    \"agentPoolProfiles\": {\n      \"type\": \"array\",\n      \"description\": \"The agent pool properties.\"\n    },\n    \"linuxProfile\": {\n      \"type\": \"object\",\n      \"description\": \"The profile for Linux VMs.\"\n    },\n    \"windowsProfile\": {\n      \"type\": \"object\",\n      \"description\": \"The profile for Windows VMs.\"\n    },\n    \"servicePrincipalProfile\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the service principal identity for the cluster.\"\n    },\n    \"addonProfiles\": {\n      \"type\": \"object\",\n      \"description\": \"The profile of managed cluster add-on.\"\n    },\n    \"nodeResourceGroup\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the resource group containing agent pool nodes.\"\n    },\n    \"enableRBAC\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable Kubernetes\
  \ RBAC.\"\n    },\n    \"enablePodSecurityPolicy\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable Kubernetes pod security policy (deprecated).\"\n    },\n    \"autoScalerProfile\": {\n      \"type\": \"object\",\n      \"description\": \"Parameters to be applied to the cluster autoscaler.\"\n    },\n    \"apiServerAccessProfile\": {\n      \"type\": \"object\",\n      \"description\": \"Access profile for managed cluster API server.\"\n    },\n    \"diskEncryptionSetID\": {\n      \"type\": \"string\",\n      \"description\": \"The resource ID of the disk encryption set.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-properties-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ManagedClusterProperties
---
