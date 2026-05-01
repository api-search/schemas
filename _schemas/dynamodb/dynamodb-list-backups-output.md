---
description: ''
layout: schema
name: ListBackupsOutput
properties_list:
- description: ''
  name: BackupSummaries
  type: array
- description: ''
  name: LastEvaluatedBackupArn
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-list-backups-output-schema.json
slug: dynamodb-list-backups-output
source_filename: dynamodb-list-backups-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListBackupsOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BackupSummaries\": {\n      \"type\": \"array\"\n    },\n    \"LastEvaluatedBackupArn\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-list-backups-output-schema.json
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: ListBackupsOutput
---
