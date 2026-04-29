---
description: The definition of a container registry operation.
layout: schema
name: OperationDefinition
properties_list:
- description: The display information for the container registry operation.
  name: display
  type: object
- description: 'Operation name: {provider}/{resource}/{operation}.'
  name: name
  type: string
- description: The origin information of the container registry operation.
  name: origin
  type: string
- description: The properties information for the container registry operation.
  name: properties
  type: object
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-operation-definition-schema.json
slug: azure-container-registry-operation-definition
source_filename: azure-container-registry-operation-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-operation-definition-schema.json\",\n  \"title\": \"OperationDefinition\",\n  \"description\": \"The definition of a container registry operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"display\": {\n      \"$ref\": \"#/definitions/OperationDisplayDefinition\",\n      \"description\": \"The display information for the container registry operation.\"\n    },\n    \"name\": {\n      \"description\": \"Operation name: {provider}/{resource}/{operation}.\",\n      \"type\": \"string\"\n    },\n    \"origin\": {\n      \"description\": \"The origin information of the container registry operation.\",\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"$ref\": \"#/definitions/OperationPropertiesDefinition\",\n      \"description\": \"The properties\
  \ information for the container registry operation.\",\n      \"x-ms-client-flatten\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-operation-definition-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: OperationDefinition
---
