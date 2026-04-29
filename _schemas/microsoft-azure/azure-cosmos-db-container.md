---
description: A Cosmos DB container (collection) resource.
layout: schema
name: Container
properties_list:
- description: The unique name that identifies the container.
  name: id
  type: string
- description: Default time-to-live in seconds. -1 means items never expire.
  name: defaultTtl
  type: integer
- description: System-generated resource ID.
  name: _rid
  type: string
- description: System-generated timestamp.
  name: _ts
  type: integer
- description: System-generated URI for the resource.
  name: _self
  type: string
- description: System-generated resource etag.
  name: _etag
  type: string
- description: Addressable path for the documents resource.
  name: _docs
  type: string
- description: Addressable path for the stored procedures resource.
  name: _sprocs
  type: string
- description: Addressable path for the triggers resource.
  name: _triggers
  type: string
- description: Addressable path for the user-defined functions resource.
  name: _udfs
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cosmos-db-container-schema.json
slug: azure-cosmos-db-container
source_filename: azure-cosmos-db-container-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Container\",\n  \"type\": \"object\",\n  \"description\": \"A Cosmos DB container (collection) resource.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name that identifies the container.\"\n    },\n    \"defaultTtl\": {\n      \"type\": \"integer\",\n      \"description\": \"Default time-to-live in seconds. -1 means items never expire.\"\n    },\n    \"_rid\": {\n      \"type\": \"string\",\n      \"description\": \"System-generated resource ID.\"\n    },\n    \"_ts\": {\n      \"type\": \"integer\",\n      \"description\": \"System-generated timestamp.\"\n    },\n    \"_self\": {\n      \"type\": \"string\",\n      \"description\": \"System-generated URI for the resource.\"\n    },\n    \"_etag\": {\n      \"type\": \"string\",\n      \"description\": \"System-generated resource etag.\"\n    },\n    \"_docs\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Addressable path for the documents resource.\"\n    },\n    \"_sprocs\": {\n      \"type\": \"string\",\n      \"description\": \"Addressable path for the stored procedures resource.\"\n    },\n    \"_triggers\": {\n      \"type\": \"string\",\n      \"description\": \"Addressable path for the triggers resource.\"\n    },\n    \"_udfs\": {\n      \"type\": \"string\",\n      \"description\": \"Addressable path for the user-defined functions resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cosmos-db-container-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Container
---
