---
description: List of Cosmos DB containers.
layout: schema
name: ContainerListResult
properties_list:
- description: ''
  name: _rid
  type: string
- description: List of containers.
  name: DocumentCollections
  type: array
- description: ''
  name: _count
  type: integer
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cosmos-db-container-list-result-schema.json
slug: azure-cosmos-db-container-list-result
source_filename: azure-cosmos-db-container-list-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContainerListResult\",\n  \"type\": \"object\",\n  \"description\": \"List of Cosmos DB containers.\",\n  \"properties\": {\n    \"_rid\": {\n      \"type\": \"string\"\n    },\n    \"DocumentCollections\": {\n      \"type\": \"array\",\n      \"description\": \"List of containers.\"\n    },\n    \"_count\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cosmos-db-container-list-result-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ContainerListResult
---
