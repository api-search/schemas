---
description: List of Cosmos DB databases.
layout: schema
name: DatabaseListResult
properties_list:
- description: The resource ID.
  name: _rid
  type: string
- description: List of databases.
  name: Databases
  type: array
- description: The number of databases returned.
  name: _count
  type: integer
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cosmos-db-database-list-result-schema.json
slug: azure-cosmos-db-database-list-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DatabaseListResult\",\n  \"type\": \"object\",\n  \"description\": \"List of Cosmos DB databases.\",\n  \"properties\": {\n    \"_rid\": {\n      \"type\": \"string\",\n      \"description\": \"The resource ID.\"\n    },\n    \"Databases\": {\n      \"type\": \"array\",\n      \"description\": \"List of databases.\"\n    },\n    \"_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of databases returned.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cosmos-db-database-list-result-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: DatabaseListResult
---
