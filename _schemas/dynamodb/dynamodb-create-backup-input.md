---
description: ''
layout: schema
name: CreateBackupInput
properties_list:
- description: ''
  name: TableName
  type: string
- description: Specified name for the backup
  name: BackupName
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-create-backup-input-schema.json
slug: dynamodb-create-backup-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateBackupInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\"\n    },\n    \"BackupName\": {\n      \"type\": \"string\",\n      \"description\": \"Specified name for the backup\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-create-backup-input-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: CreateBackupInput
---
