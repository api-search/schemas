---
description: A Cosmos DB database resource.
layout: schema
name: Database
properties_list:
- description: The unique name that identifies the database.
  name: id
  type: string
- description: System-generated resource ID.
  name: _rid
  type: string
- description: System-generated timestamp (epoch value).
  name: _ts
  type: integer
- description: System-generated URI for the resource.
  name: _self
  type: string
- description: System-generated resource etag for optimistic concurrency.
  name: _etag
  type: string
- description: System-generated addressable path for the collections resource.
  name: _colls
  type: string
- description: System-generated addressable path for the users resource.
  name: _users
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cosmos-db-database-schema.json
slug: azure-cosmos-db-database
source_filename: azure-cosmos-db-database-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Database\",\n  \"type\": \"object\",\n  \"description\": \"A Cosmos DB database resource.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name that identifies the database.\"\n    },\n    \"_rid\": {\n      \"type\": \"string\",\n      \"description\": \"System-generated resource ID.\"\n    },\n    \"_ts\": {\n      \"type\": \"integer\",\n      \"description\": \"System-generated timestamp (epoch value).\"\n    },\n    \"_self\": {\n      \"type\": \"string\",\n      \"description\": \"System-generated URI for the resource.\"\n    },\n    \"_etag\": {\n      \"type\": \"string\",\n      \"description\": \"System-generated resource etag for optimistic concurrency.\"\n    },\n    \"_colls\": {\n      \"type\": \"string\",\n      \"description\": \"System-generated addressable path for the collections resource.\"\n    },\n    \"_users\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"System-generated addressable path for the users resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cosmos-db-database-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Database
---
