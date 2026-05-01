---
description: ''
layout: schema
name: ListBackupsInput
properties_list:
- description: ''
  name: TableName
  type: string
- description: ''
  name: Limit
  type: integer
- description: ''
  name: TimeRangeLowerBound
  type: string
- description: ''
  name: TimeRangeUpperBound
  type: string
- description: ''
  name: ExclusiveStartBackupArn
  type: string
- description: ''
  name: BackupType
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-list-backups-input-schema.json
slug: dynamodb-list-backups-input
source_filename: dynamodb-list-backups-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListBackupsInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\"\n    },\n    \"Limit\": {\n      \"type\": \"integer\"\n    },\n    \"TimeRangeLowerBound\": {\n      \"type\": \"string\"\n    },\n    \"TimeRangeUpperBound\": {\n      \"type\": \"string\"\n    },\n    \"ExclusiveStartBackupArn\": {\n      \"type\": \"string\"\n    },\n    \"BackupType\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-list-backups-input-schema.json
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: ListBackupsInput
---
