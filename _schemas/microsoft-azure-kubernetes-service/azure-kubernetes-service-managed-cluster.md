---
description: Managed cluster resource representing an Azure Kubernetes Service cluster.
layout: schema
name: ManagedCluster
properties_list:
- description: 'Fully qualified resource ID for the resource. Example: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerService/managedClusters/{resourceName}'
  name: id
  type: string
- description: The name of the resource.
  name: name
  type: string
- description: 'The type of the resource. Example: Microsoft.ContainerService/managedClusters'
  name: type
  type: string
- description: The geo-location where the resource lives.
  name: location
  type: string
- description: Resource tags.
  name: tags
  type: object
- description: This is primarily used to expose different UI experiences in the portal for different kinds.
  name: kind
  type: string
provider_name: Azure Kubernetes Service
provider_slug: microsoft-azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-schema.json
slug: azure-kubernetes-service-managed-cluster
source_filename: azure-kubernetes-service-managed-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedCluster\",\n  \"type\": \"object\",\n  \"description\": \"Managed cluster resource representing an Azure Kubernetes Service cluster.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified resource ID for the resource. Example: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerService/managedClusters/{resourceName}\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the resource.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the resource. Example: Microsoft.ContainerService/managedClusters\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The geo-location where the resource lives.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"\
  Resource tags.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"This is primarily used to expose different UI experiences in the portal for different kinds.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedCluster
---
