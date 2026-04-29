---
description: The display information for a container registry operation.
layout: schema
name: OperationDisplayDefinition
properties_list:
- description: The description for the operation.
  name: description
  type: string
- description: The operation that users can perform.
  name: operation
  type: string
- description: 'The resource provider name: Microsoft.ContainerRegistry.'
  name: provider
  type: string
- description: The resource on which the operation is performed.
  name: resource
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-operation-display-definition-schema.json
slug: azure-container-registry-operation-display-definition
source_filename: azure-container-registry-operation-display-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-operation-display-definition-schema.json\",\n  \"title\": \"OperationDisplayDefinition\",\n  \"description\": \"The display information for a container registry operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"The description for the operation.\",\n      \"type\": \"string\"\n    },\n    \"operation\": {\n      \"description\": \"The operation that users can perform.\",\n      \"type\": \"string\"\n    },\n    \"provider\": {\n      \"description\": \"The resource provider name: Microsoft.ContainerRegistry.\",\n      \"type\": \"string\"\n    },\n    \"resource\": {\n      \"description\": \"The resource on which the operation is performed.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-operation-display-definition-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: OperationDisplayDefinition
---
