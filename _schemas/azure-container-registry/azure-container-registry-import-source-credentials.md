---
description: ImportSourceCredentials schema from Azure Container Registry API
layout: schema
name: ImportSourceCredentials
properties_list:
- description: The password used to authenticate with the source registry.
  name: password
  type: string
- description: The username to authenticate with the source registry.
  name: username
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-import-source-credentials-schema.json
slug: azure-container-registry-import-source-credentials
source_filename: azure-container-registry-import-source-credentials-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-import-source-credentials-schema.json\",\n  \"title\": \"ImportSourceCredentials\",\n  \"description\": \"ImportSourceCredentials schema from Azure Container Registry API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"password\": {\n      \"description\": \"The password used to authenticate with the source registry.\",\n      \"type\": \"string\"\n    },\n    \"username\": {\n      \"description\": \"The username to authenticate with the source registry.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"password\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-import-source-credentials-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: ImportSourceCredentials
---
