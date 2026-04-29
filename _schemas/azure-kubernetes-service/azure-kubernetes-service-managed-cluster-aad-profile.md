---
description: Azure Active Directory configuration for integration with AKS.
layout: schema
name: ManagedClusterAADProfile
properties_list:
- description: Whether to enable managed AAD.
  name: managed
  type: boolean
- description: Whether to enable Azure RBAC for Kubernetes authorization.
  name: enableAzureRBAC
  type: boolean
- description: The list of AAD group object IDs that will have admin role of the cluster.
  name: adminGroupObjectIDs
  type: array
- description: (DEPRECATED) The client AAD application ID. Used for legacy/non-managed AAD.
  name: clientAppID
  type: string
- description: (DEPRECATED) The server AAD application ID. Used for legacy/non-managed AAD.
  name: serverAppID
  type: string
- description: (DEPRECATED) The server AAD application secret. Used for legacy/non-managed AAD.
  name: serverAppSecret
  type: string
- description: The AAD tenant ID to use for authentication. If not specified, will use the tenant of the deployment subscription.
  name: tenantID
  type: string
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-aad-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-aad-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterAADProfile\",\n  \"type\": \"object\",\n  \"description\": \"Azure Active Directory configuration for integration with AKS.\",\n  \"properties\": {\n    \"managed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable managed AAD.\"\n    },\n    \"enableAzureRBAC\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable Azure RBAC for Kubernetes authorization.\"\n    },\n    \"adminGroupObjectIDs\": {\n      \"type\": \"array\",\n      \"description\": \"The list of AAD group object IDs that will have admin role of the cluster.\"\n    },\n    \"clientAppID\": {\n      \"type\": \"string\",\n      \"description\": \"(DEPRECATED) The client AAD application ID. Used for legacy/non-managed AAD.\"\n    },\n    \"serverAppID\": {\n      \"type\": \"string\",\n      \"description\": \"(DEPRECATED) The server AAD application ID. Used for legacy/non-managed\
  \ AAD.\"\n    },\n    \"serverAppSecret\": {\n      \"type\": \"string\",\n      \"description\": \"(DEPRECATED) The server AAD application secret. Used for legacy/non-managed AAD.\"\n    },\n    \"tenantID\": {\n      \"type\": \"string\",\n      \"description\": \"The AAD tenant ID to use for authentication. If not specified, will use the tenant of the deployment subscription.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-aad-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterAADProfile
---
