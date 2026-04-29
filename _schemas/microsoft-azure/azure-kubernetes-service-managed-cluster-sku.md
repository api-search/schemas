---
description: The SKU of a managed cluster.
layout: schema
name: ManagedClusterSKU
properties_list:
- description: The name of the managed cluster SKU.
  name: name
  type: string
- description: The tier of the managed cluster SKU.
  name: tier
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-kubernetes-service-managed-cluster-sku-schema.json
slug: azure-kubernetes-service-managed-cluster-sku
source_filename: azure-kubernetes-service-managed-cluster-sku-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterSKU\",\n  \"type\": \"object\",\n  \"description\": \"The SKU of a managed cluster.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the managed cluster SKU.\"\n    },\n    \"tier\": {\n      \"type\": \"string\",\n      \"description\": \"The tier of the managed cluster SKU.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-sku-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ManagedClusterSKU
---
