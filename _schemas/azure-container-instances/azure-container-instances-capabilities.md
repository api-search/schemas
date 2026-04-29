---
description: The regional capabilities.
layout: schema
name: Capabilities
properties_list:
- description: The supported capabilities.
  name: capabilities
  type: object
- description: The GPU sku that this capability describes.
  name: gpu
  type: string
- description: The ip address type that this capability describes.
  name: ipAddressType
  type: string
- description: The resource location.
  name: location
  type: string
- description: The OS type that this capability describes.
  name: osType
  type: string
- description: The resource type that this capability describes.
  name: resourceType
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-capabilities-schema.json
slug: azure-container-instances-capabilities
source_filename: azure-container-instances-capabilities-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-capabilities-schema.json\",\n  \"title\": \"Capabilities\",\n  \"description\": \"The regional capabilities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"capabilities\": {\n      \"description\": \"The supported capabilities.\",\n      \"properties\": {\n        \"maxCpu\": {\n          \"description\": \"The maximum allowed CPU request in cores.\",\n          \"readOnly\": true,\n          \"type\": \"number\"\n        },\n        \"maxGpuCount\": {\n          \"description\": \"The maximum allowed GPU count.\",\n          \"readOnly\": true,\n          \"type\": \"number\"\n        },\n        \"maxMemoryInGB\": {\n          \"description\": \"The maximum allowed memory request in GB.\",\n          \"readOnly\": true,\n          \"type\": \"number\"\n  \
  \      }\n      },\n      \"readOnly\": true,\n      \"type\": \"object\"\n    },\n    \"gpu\": {\n      \"description\": \"The GPU sku that this capability describes.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"ipAddressType\": {\n      \"description\": \"The ip address type that this capability describes.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"location\": {\n      \"description\": \"The resource location.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"osType\": {\n      \"description\": \"The OS type that this capability describes.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"resourceType\": {\n      \"description\": \"The resource type that this capability describes.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-capabilities-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: Capabilities
---
