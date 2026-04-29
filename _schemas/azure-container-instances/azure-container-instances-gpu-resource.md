---
description: The GPU resource.
layout: schema
name: GpuResource
properties_list:
- description: The count of the GPU resource.
  name: count
  type: integer
- description: The SKU of the GPU resource.
  name: sku
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-gpu-resource-schema.json
slug: azure-container-instances-gpu-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-gpu-resource-schema.json\",\n  \"title\": \"GpuResource\",\n  \"description\": \"The GPU resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"description\": \"The count of the GPU resource.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"sku\": {\n      \"description\": \"The SKU of the GPU resource.\",\n      \"enum\": [\n        \"K80\",\n        \"P100\",\n        \"V100\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"GpuSku\"\n      }\n    }\n  },\n  \"required\": [\n    \"count\",\n    \"sku\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-gpu-resource-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: GpuResource
---
