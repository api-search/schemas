---
description: The container group list response that contains the container group properties.
layout: schema
name: ContainerGroupListResult
properties_list:
- description: The URI to fetch the next page of container groups.
  name: nextLink
  type: string
- description: The list of container groups.
  name: value
  type: array
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-container-group-list-result-schema.json
slug: azure-container-instances-container-group-list-result
source_filename: azure-container-instances-container-group-list-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-group-list-result-schema.json\",\n  \"title\": \"ContainerGroupListResult\",\n  \"description\": \"The container group list response that contains the container group properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextLink\": {\n      \"description\": \"The URI to fetch the next page of container groups.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The list of container groups.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/ContainerGroup\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-group-list-result-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ContainerGroupListResult
---
