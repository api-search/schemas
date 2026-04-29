---
description: A Cosmos DB stored procedure.
layout: schema
name: StoredProcedure
properties_list:
- description: The unique name of the stored procedure.
  name: id
  type: string
- description: The body of the stored procedure (JavaScript function).
  name: body
  type: string
- description: ''
  name: _rid
  type: string
- description: ''
  name: _ts
  type: integer
- description: ''
  name: _self
  type: string
- description: ''
  name: _etag
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cosmos-db-stored-procedure-schema.json
slug: azure-cosmos-db-stored-procedure
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StoredProcedure\",\n  \"type\": \"object\",\n  \"description\": \"A Cosmos DB stored procedure.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name of the stored procedure.\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"The body of the stored procedure (JavaScript function).\"\n    },\n    \"_rid\": {\n      \"type\": \"string\"\n    },\n    \"_ts\": {\n      \"type\": \"integer\"\n    },\n    \"_self\": {\n      \"type\": \"string\"\n    },\n    \"_etag\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cosmos-db-stored-procedure-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: StoredProcedure
---
