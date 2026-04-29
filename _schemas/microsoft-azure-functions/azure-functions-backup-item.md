---
description: Backup description.
layout: schema
name: BackupItem
properties_list:
- description: BackupItem resource specific properties
  name: properties
  type: object
- description: Kind of resource.
  name: kind
  type: string
provider_name: Microsoft Azure Functions
provider_slug: microsoft-azure-functions
schema_file: json-schema/azure-functions-backup-item-schema.json
slug: azure-functions-backup-item
source_filename: azure-functions-backup-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-backup-item-schema.json\",\n  \"title\": \"BackupItem\",\n  \"description\": \"Backup description.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/BackupItemProperties\",\n      \"description\": \"BackupItem resource specific properties\",\n      \"x-ms-client-flatten\": true\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Kind of resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-backup-item-schema.json
tags:
- Azure
- Cloud
- Compute
- Event-Driven
- Microsoft
- Serverless
title: BackupItem
---
