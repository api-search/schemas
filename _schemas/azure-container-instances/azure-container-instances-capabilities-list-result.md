---
description: The response containing list of capabilities.
layout: schema
name: CapabilitiesListResult
properties_list:
- description: The URI to fetch the next page of capabilities.
  name: nextLink
  type: string
- description: The list of capabilities.
  name: value
  type: array
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-capabilities-list-result-schema.json
slug: azure-container-instances-capabilities-list-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-capabilities-list-result-schema.json\",\n  \"title\": \"CapabilitiesListResult\",\n  \"description\": \"The response containing list of capabilities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextLink\": {\n      \"description\": \"The URI to fetch the next page of capabilities.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The list of capabilities.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Capabilities\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-capabilities-list-result-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: CapabilitiesListResult
---
