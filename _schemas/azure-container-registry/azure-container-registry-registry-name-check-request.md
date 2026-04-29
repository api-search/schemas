---
description: A request to check whether a container registry name is available.
layout: schema
name: RegistryNameCheckRequest
properties_list:
- description: The name of the container registry.
  name: name
  type: string
- description: The resource type of the container registry. This field must be set to 'Microsoft.ContainerRegistry/registries'.
  name: type
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-registry-name-check-request-schema.json
slug: azure-container-registry-registry-name-check-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-registry-name-check-request-schema.json\",\n  \"title\": \"RegistryNameCheckRequest\",\n  \"description\": \"A request to check whether a container registry name is available.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"The name of the container registry.\",\n      \"maxLength\": 50,\n      \"minLength\": 5,\n      \"pattern\": \"^[a-zA-Z0-9]*$\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The resource type of the container registry. This field must be set to 'Microsoft.ContainerRegistry/registries'.\",\n      \"enum\": [\n        \"Microsoft.ContainerRegistry/registries\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\"\
  : \"ContainerRegistryResourceType\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-registry-name-check-request-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: RegistryNameCheckRequest
---
