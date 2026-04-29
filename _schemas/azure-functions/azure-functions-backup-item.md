---
description: Backup description.
layout: schema
name: BackupItem
properties_list:
- description: BackupItem resource specific properties
  name: properties
  type: object
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-backup-item-schema.json
slug: azure-functions-backup-item
source_filename: azure-functions-backup-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-backup-item-schema.json\",\n  \"title\": \"BackupItem\",\n  \"description\": \"Backup description.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"description\": \"BackupItem resource specific properties\",\n      \"properties\": {\n        \"blobName\": {\n          \"description\": \"Name of the blob which contains data for this backup.\",\n          \"readOnly\": true,\n          \"type\": \"string\"\n        },\n        \"correlationId\": {\n          \"description\": \"Unique correlation identifier. Please use this along with the timestamp while communicating with Azure support.\",\n          \"readOnly\": true,\n          \"type\": \"string\"\n        },\n        \"created\": {\n          \"description\": \"Timestamp of the backup creation.\",\n  \
  \        \"format\": \"date-time\",\n          \"readOnly\": true,\n          \"type\": \"string\"\n        },\n        \"databases\": {\n          \"description\": \"List of databases included in the backup.\",\n          \"items\": {\n            \"$ref\": \"#/definitions/DatabaseBackupSetting\"\n          },\n          \"readOnly\": true,\n          \"type\": \"array\"\n        },\n        \"finishedTimeStamp\": {\n          \"description\": \"Timestamp when this backup finished.\",\n          \"format\": \"date-time\",\n          \"readOnly\": true,\n          \"type\": \"string\"\n        },\n        \"id\": {\n          \"description\": \"Id of the backup.\",\n          \"format\": \"int32\",\n          \"readOnly\": true,\n          \"type\": \"integer\",\n          \"x-ms-client-name\": \"BackupId\"\n        },\n        \"lastRestoreTimeStamp\": {\n          \"description\": \"Timestamp of a last restore operation which used this backup.\",\n          \"format\": \"date-time\"\
  ,\n          \"readOnly\": true,\n          \"type\": \"string\"\n        },\n        \"log\": {\n          \"description\": \"Details regarding this backup. Might contain an error message.\",\n          \"readOnly\": true,\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"description\": \"Name of this backup.\",\n          \"readOnly\": true,\n          \"type\": \"string\"\n        },\n        \"scheduled\": {\n          \"description\": \"True if this backup has been created due to a schedule being triggered.\",\n          \"readOnly\": true,\n          \"type\": \"boolean\"\n        },\n        \"sizeInBytes\": {\n          \"description\": \"Size of the backup in bytes.\",\n          \"format\": \"int64\",\n          \"readOnly\": true,\n          \"type\": \"integer\"\n        },\n        \"status\": {\n          \"description\": \"Backup status.\",\n          \"enum\": [\n            \"InProgress\",\n            \"Failed\",\n            \"Succeeded\"\
  ,\n            \"TimedOut\",\n            \"Created\",\n            \"Skipped\",\n            \"PartiallySucceeded\",\n            \"DeleteInProgress\",\n            \"DeleteFailed\",\n            \"Deleted\"\n          ],\n          \"readOnly\": true,\n          \"type\": \"string\",\n          \"x-ms-enum\": {\n            \"modelAsString\": false,\n            \"name\": \"BackupItemStatus\"\n          }\n        },\n        \"storageAccountUrl\": {\n          \"description\": \"SAS URL for the storage account container which contains this backup.\",\n          \"readOnly\": true,\n          \"type\": \"string\"\n        },\n        \"websiteSizeInBytes\": {\n          \"description\": \"Size of the original web app which has been backed up.\",\n          \"format\": \"int64\",\n          \"readOnly\": true,\n          \"type\": \"integer\"\n        }\n      },\n      \"x-ms-client-flatten\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-backup-item-schema.json
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: BackupItem
---
