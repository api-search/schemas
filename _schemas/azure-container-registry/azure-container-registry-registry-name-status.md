---
description: The result of a request to check the availability of a container registry name.
layout: schema
name: RegistryNameStatus
properties_list:
- description: If any, the error message that provides more detail for the reason that the name is not available.
  name: message
  type: string
- description: The value that indicates whether the name is available.
  name: nameAvailable
  type: boolean
- description: If any, the reason that the name is not available.
  name: reason
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-registry-name-status-schema.json
slug: azure-container-registry-registry-name-status
source_filename: azure-container-registry-registry-name-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-registry-name-status-schema.json\",\n  \"title\": \"RegistryNameStatus\",\n  \"description\": \"The result of a request to check the availability of a container registry name.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"description\": \"If any, the error message that provides more detail for the reason that the name is not available.\",\n      \"type\": \"string\"\n    },\n    \"nameAvailable\": {\n      \"description\": \"The value that indicates whether the name is available.\",\n      \"type\": \"boolean\"\n    },\n    \"reason\": {\n      \"description\": \"If any, the reason that the name is not available.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-registry-name-status-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: RegistryNameStatus
---
