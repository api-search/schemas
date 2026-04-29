---
description: The SKU of a Managed Cluster.
layout: schema
name: ManagedClusterSKU
properties_list:
- description: The name of a managed cluster SKU.
  name: name
  type: string
- description: If not specified, the default is Free. See AKS Pricing Tier for more details.
  name: tier
  type: string
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-sku-schema.json
slug: azure-kubernetes-service-managed-cluster-sku
source_filename: azure-kubernetes-service-managed-cluster-sku-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterSKU\",\n  \"type\": \"object\",\n  \"description\": \"The SKU of a Managed Cluster.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of a managed cluster SKU.\"\n    },\n    \"tier\": {\n      \"type\": \"string\",\n      \"description\": \"If not specified, the default is Free. See AKS Pricing Tier for more details.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-sku-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterSKU
---
