---
description: The response from the ListCredentials operation.
layout: schema
name: RegistryListCredentialsResult
properties_list:
- description: The list of passwords for a container registry.
  name: passwords
  type: array
- description: The username for a container registry.
  name: username
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-registry-list-credentials-result-schema.json
slug: azure-container-registry-registry-list-credentials-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-registry-list-credentials-result-schema.json\",\n  \"title\": \"RegistryListCredentialsResult\",\n  \"description\": \"The response from the ListCredentials operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"passwords\": {\n      \"description\": \"The list of passwords for a container registry.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/RegistryPassword\"\n      },\n      \"type\": \"array\"\n    },\n    \"username\": {\n      \"description\": \"The username for a container registry.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-registry-list-credentials-result-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: RegistryListCredentialsResult
---
