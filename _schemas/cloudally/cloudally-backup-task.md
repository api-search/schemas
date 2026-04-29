---
description: Schema for a CloudAlly backup task. A backup task represents the configuration that protects a specific SaaS workload (Microsoft 365 mailbox, Google Workspace user, Salesforce org, Box account, or Dropbox account). The task carries identifying metadata, scheduling info, status, and links to the most recent backup snapshot.
layout: schema
name: CloudAlly Backup Task
properties_list:
- description: Unique identifier of the backup task.
  name: id
  type: string
- description: Human-readable label for the task.
  name: name
  type: string
- description: Workload type protected by the task.
  name: type
  type: string
- description: Current backup status (for example, success, failed, in_progress, paused).
  name: status
  type: string
- description: Timestamp of the most recent successful backup.
  name: lastBackup
  type:
  - string
  - 'null'
- description: Time the task was created.
  name: createdAt
  type: string
- description: Total backed-up data size in bytes for the task.
  name: size
  type:
  - integer
  - 'null'
- description: Backup schedule configuration.
  name: schedule
  type: object
provider_name: CloudAlly
provider_slug: cloudally
schema_file: json-schema/cloudally-backup-task-schema.json
slug: cloudally-backup-task
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.cloudally.com/schemas/backup-task.json\",\n  \"title\": \"CloudAlly Backup Task\",\n  \"description\": \"Schema for a CloudAlly backup task. A backup task represents the configuration that protects a specific SaaS workload (Microsoft 365 mailbox, Google Workspace user, Salesforce org, Box account, or Dropbox account). The task carries identifying metadata, scheduling info, status, and links to the most recent backup snapshot.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the backup task.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable label for the task.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Workload type protected by the task.\",\n      \"enum\": [\"\
  MS365\", \"GOOGLE_WORKSPACE\", \"SALESFORCE\", \"BOX\", \"DROPBOX\", \"SHAREPOINT\", \"ONEDRIVE\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current backup status (for example, success, failed, in_progress, paused).\",\n      \"enum\": [\"success\", \"failed\", \"in_progress\", \"paused\", \"pending\"]\n    },\n    \"lastBackup\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the most recent successful backup.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time the task was created.\"\n    },\n    \"size\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Total backed-up data size in bytes for the task.\"\n    },\n    \"schedule\": {\n      \"type\": \"object\",\n      \"description\": \"Backup schedule configuration.\",\n      \"properties\": {\n        \"frequency\": {\"type\": \"string\"\
  , \"enum\": [\"daily\", \"every_3_hours\", \"manual\"]},\n        \"timezone\": {\"type\": \"string\"}\n      }\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudally/refs/heads/main/json-schema/cloudally-backup-task-schema.json
tags:
- Backup
- Box
- Data Protection
- Disaster Recovery
- Dropbox
- Google Workspace
- Microsoft 365
- OpenText
- SaaS Backup
- Salesforce
title: CloudAlly Backup Task
---
