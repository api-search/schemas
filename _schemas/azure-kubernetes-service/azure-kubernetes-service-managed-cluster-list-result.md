---
description: The response from the List Managed Clusters operation.
layout: schema
name: ManagedClusterListResult
properties_list:
- description: The list of managed clusters.
  name: value
  type: array
- description: The URL to get the next set of managed cluster results.
  name: nextLink
  type: string
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-list-result-schema.json
slug: azure-kubernetes-service-managed-cluster-list-result
source_filename: azure-kubernetes-service-managed-cluster-list-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterListResult\",\n  \"type\": \"object\",\n  \"description\": \"The response from the List Managed Clusters operation.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"The list of managed clusters.\"\n    },\n    \"nextLink\": {\n      \"type\": \"string\",\n      \"description\": \"The URL to get the next set of managed cluster results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-list-result-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterListResult
---
