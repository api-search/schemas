---
description: An automatic or user-initiated backup of an Amazon FSx file system.
layout: schema
name: Backup
properties_list:
- description: Unique ID of the backup.
  name: BackupId
  type: string
- description: Current lifecycle state.
  name: Lifecycle
  type: string
- description: Type of backup.
  name: Type
  type: string
- description: ''
  name: CreationTime
  type: string
- description: The file system that was backed up.
  name: FileSystem
  type: object
- description: ''
  name: KmsKeyId
  type: string
- description: ''
  name: ResourceARN
  type: string
- description: ''
  name: Tags
  type: array
- description: ''
  name: OwnerId
  type: string
- description: ''
  name: SourceBackupId
  type: string
provider_name: Amazon FSx
provider_slug: amazon-fsx
schema_file: json-schema/amazon-fsx-backup-schema.json
slug: amazon-fsx-backup
source_filename: amazon-fsx-backup-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fsx/refs/heads/main/json-schema/amazon-fsx-backup-schema.json\",\n  \"title\": \"Backup\",\n  \"description\": \"An automatic or user-initiated backup of an Amazon FSx file system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BackupId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ID of the backup.\"\n    },\n    \"Lifecycle\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AVAILABLE\",\n        \"CREATING\",\n        \"TRANSFERRING\",\n        \"DELETED\",\n        \"FAILED\",\n        \"PENDING\",\n        \"COPYING\"\n      ],\n      \"description\": \"Current lifecycle state.\"\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AUTOMATIC\",\n        \"USER_INITIATED\",\n        \"AWS_BACKUP\"\n      ],\n      \"description\": \"Type of backup.\"\n    },\n  \
  \  \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"FileSystem\": {\n      \"type\": \"object\",\n      \"description\": \"The file system that was backed up.\"\n    },\n    \"KmsKeyId\": {\n      \"type\": \"string\"\n    },\n    \"ResourceARN\": {\n      \"type\": \"string\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"OwnerId\": {\n      \"type\": \"string\"\n    },\n    \"SourceBackupId\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"BackupId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fsx/refs/heads/main/json-schema/amazon-fsx-backup-schema.json
tags:
- File Systems
- Lustre
- NetApp
- OpenZFS
- Storage
- Windows
title: Backup
---
