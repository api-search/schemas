---
description: The result of a request to list container registries.
layout: schema
name: RegistryListResult
properties_list:
- description: The URI that can be used to request the next list of container registries.
  name: nextLink
  type: string
- description: The list of container registries. Since this list may be incomplete, the nextLink field should be used to request the next list of container registries.
  name: value
  type: array
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-registry-list-result-schema.json
slug: azure-container-registry-registry-list-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-registry-list-result-schema.json\",\n  \"title\": \"RegistryListResult\",\n  \"description\": \"The result of a request to list container registries.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextLink\": {\n      \"description\": \"The URI that can be used to request the next list of container registries.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The list of container registries. Since this list may be incomplete, the nextLink field should be used to request the next list of container registries.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Registry\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-registry-list-result-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: RegistryListResult
---
