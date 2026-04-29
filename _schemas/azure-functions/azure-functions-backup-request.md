---
description: Description of a backup which will be performed.
layout: schema
name: BackupRequest
properties_list:
- description: BackupRequest resource specific properties
  name: properties
  type: object
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-backup-request-schema.json
slug: azure-functions-backup-request
source_filename: azure-functions-backup-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-backup-request-schema.json\",\n  \"title\": \"BackupRequest\",\n  \"description\": \"Description of a backup which will be performed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"description\": \"BackupRequest resource specific properties\",\n      \"properties\": {\n        \"backupName\": {\n          \"description\": \"Name of the backup.\",\n          \"type\": \"string\"\n        },\n        \"backupSchedule\": {\n          \"$ref\": \"#/definitions/BackupSchedule\",\n          \"description\": \"Schedule for the backup if it is executed periodically.\"\n        },\n        \"databases\": {\n          \"description\": \"Databases included in the backup.\",\n          \"items\": {\n            \"$ref\": \"#/definitions/DatabaseBackupSetting\"\n  \
  \        },\n          \"type\": \"array\"\n        },\n        \"enabled\": {\n          \"description\": \"True if the backup schedule is enabled (must be included in that case), false if the backup schedule should be disabled.\",\n          \"type\": \"boolean\"\n        },\n        \"storageAccountUrl\": {\n          \"description\": \"SAS URL to the container.\",\n          \"type\": \"string\"\n        }\n      },\n      \"required\": [\n        \"storageAccountUrl\"\n      ],\n      \"x-ms-client-flatten\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-backup-request-schema.json
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: BackupRequest
---
