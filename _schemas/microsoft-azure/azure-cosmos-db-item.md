---
description: A Cosmos DB item (document).
layout: schema
name: Item
properties_list:
- description: The unique identifier of the item.
  name: id
  type: string
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
- description: Addressable path for the attachments resource.
  name: _attachments
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cosmos-db-item-schema.json
slug: azure-cosmos-db-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Item\",\n  \"type\": \"object\",\n  \"description\": \"A Cosmos DB item (document).\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the item.\"\n    },\n    \"_rid\": {\n      \"type\": \"string\",\n      \"description\": \"System-generated resource ID.\"\n    },\n    \"_ts\": {\n      \"type\": \"integer\",\n      \"description\": \"System-generated timestamp.\"\n    },\n    \"_self\": {\n      \"type\": \"string\",\n      \"description\": \"System-generated URI for the resource.\"\n    },\n    \"_etag\": {\n      \"type\": \"string\",\n      \"description\": \"System-generated resource etag.\"\n    },\n    \"_attachments\": {\n      \"type\": \"string\",\n      \"description\": \"Addressable path for the attachments resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cosmos-db-item-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Item
---
