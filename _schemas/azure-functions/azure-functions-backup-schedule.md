---
description: Description of a backup schedule. Describes how often should be the backup performed and what should be the retention policy.
layout: schema
name: BackupSchedule
properties_list:
- description: How often the backup should be executed (e.g. for weekly backup, this should be set to 7 and FrequencyUnit should be set to Day)
  name: frequencyInterval
  type: integer
- description: The unit of time for how often the backup should be executed (e.g. for weekly backup, this should be set to Day and FrequencyInterval should be set to 7)
  name: frequencyUnit
  type: string
- description: True if the retention policy should always keep at least one backup in the storage account, regardless how old it is; false otherwise.
  name: keepAtLeastOneBackup
  type: boolean
- description: Last time when this schedule was triggered.
  name: lastExecutionTime
  type: string
- description: After how many days backups should be deleted.
  name: retentionPeriodInDays
  type: integer
- description: When the schedule should start working.
  name: startTime
  type: string
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-backup-schedule-schema.json
slug: azure-functions-backup-schedule
source_filename: azure-functions-backup-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-backup-schedule-schema.json\",\n  \"title\": \"BackupSchedule\",\n  \"description\": \"Description of a backup schedule. Describes how often should be the backup performed and what should be the retention policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"frequencyInterval\": {\n      \"default\": 7,\n      \"description\": \"How often the backup should be executed (e.g. for weekly backup, this should be set to 7 and FrequencyUnit should be set to Day)\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"frequencyUnit\": {\n      \"default\": \"Day\",\n      \"description\": \"The unit of time for how often the backup should be executed (e.g. for weekly backup, this should be set to Day and FrequencyInterval should be set to 7)\",\n      \"enum\": [\n\
  \        \"Day\",\n        \"Hour\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\": \"FrequencyUnit\"\n      }\n    },\n    \"keepAtLeastOneBackup\": {\n      \"default\": true,\n      \"description\": \"True if the retention policy should always keep at least one backup in the storage account, regardless how old it is; false otherwise.\",\n      \"type\": \"boolean\"\n    },\n    \"lastExecutionTime\": {\n      \"description\": \"Last time when this schedule was triggered.\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"retentionPeriodInDays\": {\n      \"default\": 30,\n      \"description\": \"After how many days backups should be deleted.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"startTime\": {\n      \"description\": \"When the schedule should start working.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\
  \n    }\n  },\n  \"required\": [\n    \"frequencyInterval\",\n    \"frequencyUnit\",\n    \"keepAtLeastOneBackup\",\n    \"retentionPeriodInDays\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-backup-schedule-schema.json
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: BackupSchedule
---
