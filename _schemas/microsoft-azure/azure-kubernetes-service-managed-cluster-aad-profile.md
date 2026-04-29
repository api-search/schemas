---
description: AAD profile for the managed cluster.
layout: schema
name: ManagedClusterAADProfile
properties_list:
- description: Whether to enable managed AAD.
  name: managed
  type: boolean
- description: Whether to enable Azure RBAC for Kubernetes authorization.
  name: enableAzureRBAC
  type: boolean
- description: The list of AAD group object IDs for cluster admin role.
  name: adminGroupObjectIDs
  type: array
- description: The AAD tenant ID for authentication.
  name: tenantID
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-kubernetes-service-managed-cluster-aad-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-aad-profile
source_filename: azure-kubernetes-service-managed-cluster-aad-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterAADProfile\",\n  \"type\": \"object\",\n  \"description\": \"AAD profile for the managed cluster.\",\n  \"properties\": {\n    \"managed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable managed AAD.\"\n    },\n    \"enableAzureRBAC\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable Azure RBAC for Kubernetes authorization.\"\n    },\n    \"adminGroupObjectIDs\": {\n      \"type\": \"array\",\n      \"description\": \"The list of AAD group object IDs for cluster admin role.\"\n    },\n    \"tenantID\": {\n      \"type\": \"string\",\n      \"description\": \"The AAD tenant ID for authentication.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-aad-profile-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ManagedClusterAADProfile
---
