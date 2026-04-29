---
description: Collection of backup items.
layout: schema
name: BackupItemCollection
properties_list:
- description: Link to next page of resources.
  name: nextLink
  type: string
- description: Collection of resources.
  name: value
  type: array
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-backup-item-collection-schema.json
slug: azure-functions-backup-item-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-backup-item-collection-schema.json\",\n  \"title\": \"BackupItemCollection\",\n  \"description\": \"Collection of backup items.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextLink\": {\n      \"description\": \"Link to next page of resources.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"Collection of resources.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/BackupItem\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-backup-item-collection-schema.json
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: BackupItemCollection
---
