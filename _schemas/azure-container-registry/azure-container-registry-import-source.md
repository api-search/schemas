---
description: ImportSource schema from Azure Container Registry API
layout: schema
name: ImportSource
properties_list:
- description: Credentials used when importing from a registry uri.
  name: credentials
  type: object
- description: The address of the source registry (e.g. 'mcr.microsoft.com').
  name: registryUri
  type: string
- description: The resource identifier of the source Azure Container Registry.
  name: resourceId
  type: string
- description: Repository name of the source image. Specify an image by repository ('hello-world'). This will use the 'latest' tag. Specify an image by tag ('hello-world:latest'). Specify an image by sha256-based ma
  name: sourceImage
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-import-source-schema.json
slug: azure-container-registry-import-source
source_filename: azure-container-registry-import-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-import-source-schema.json\",\n  \"title\": \"ImportSource\",\n  \"description\": \"ImportSource schema from Azure Container Registry API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"credentials\": {\n      \"$ref\": \"#/definitions/ImportSourceCredentials\",\n      \"description\": \"Credentials used when importing from a registry uri.\"\n    },\n    \"registryUri\": {\n      \"description\": \"The address of the source registry (e.g. 'mcr.microsoft.com').\",\n      \"type\": \"string\"\n    },\n    \"resourceId\": {\n      \"description\": \"The resource identifier of the source Azure Container Registry.\",\n      \"type\": \"string\"\n    },\n    \"sourceImage\": {\n      \"description\": \"Repository name of the source image.\\r\\nSpecify an image by repository\
  \ ('hello-world'). This will use the 'latest' tag.\\r\\nSpecify an image by tag ('hello-world:latest').\\r\\nSpecify an image by sha256-based manifest digest ('hello-world@sha256:abc123').\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"sourceImage\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-import-source-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: ImportSource
---
