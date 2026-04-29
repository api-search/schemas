---
description: Represents an AWS Backup plan with its associated rules, schedule, and lifecycle configuration.
layout: schema
name: Amazon Backup Plan
properties_list:
- description: The Amazon Resource Name (ARN) of the backup plan.
  name: backupPlanArn
  type: string
- description: Uniquely identifies a backup plan.
  name: backupPlanId
  type: string
- description: The display name of a backup plan.
  name: backupPlanName
  type: string
- description: The date and time the resource backup plan was created.
  name: creationDate
  type: string
- description: The last time a job to back up resources was run with this rule.
  name: lastExecutionDate
  type: string
- description: An array of BackupRule objects, each of which specifies a scheduled task to back up a selection of resources.
  name: rules
  type: array
- description: Advanced backup settings for the backup plan.
  name: advancedBackupSettings
  type: array
provider_name: Amazon Backup
provider_slug: amazon-backup
schema_file: json-schema/amazon-backup-plan-schema.json
slug: amazon-backup-plan
source_filename: amazon-backup-plan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/amazon/backup/backup-plan.json\",\n  \"title\": \"Amazon Backup Plan\",\n  \"description\": \"Represents an AWS Backup plan with its associated rules, schedule, and lifecycle configuration.\",\n  \"type\": \"object\",\n  \"required\": [\"backupPlanName\", \"rules\"],\n  \"properties\": {\n    \"backupPlanArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the backup plan.\",\n      \"pattern\": \"^arn:aws:backup:[a-z0-9-]+:[0-9]{12}:backup-plan:.+$\"\n    },\n    \"backupPlanId\": {\n      \"type\": \"string\",\n      \"description\": \"Uniquely identifies a backup plan.\"\n    },\n    \"backupPlanName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of a backup plan.\",\n      \"minLength\": 1,\n      \"maxLength\": 50\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n   \
  \   \"format\": \"date-time\",\n      \"description\": \"The date and time the resource backup plan was created.\"\n    },\n    \"lastExecutionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The last time a job to back up resources was run with this rule.\"\n    },\n    \"rules\": {\n      \"type\": \"array\",\n      \"description\": \"An array of BackupRule objects, each of which specifies a scheduled task to back up a selection of resources.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"ruleName\", \"targetBackupVaultName\"],\n        \"properties\": {\n          \"ruleName\": {\n            \"type\": \"string\",\n            \"description\": \"A display name for a backup rule.\"\n          },\n          \"targetBackupVaultName\": {\n            \"type\": \"string\",\n            \"description\": \"The name of a logical container where backups are stored.\"\n          },\n          \"scheduleExpression\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"A cron expression in UTC specifying when Backup initiates a backup job.\"\n          },\n          \"startWindowMinutes\": {\n            \"type\": \"integer\",\n            \"description\": \"A value in minutes after a backup is scheduled before a job will be canceled.\"\n          },\n          \"completionWindowMinutes\": {\n            \"type\": \"integer\",\n            \"description\": \"A value in minutes after a backup job is successfully started before it must be completed.\"\n          },\n          \"lifecycle\": {\n            \"type\": \"object\",\n            \"description\": \"The lifecycle defines when a protected resource is transitioned to cold storage and when it expires.\",\n            \"properties\": {\n              \"moveToColdStorageAfterDays\": {\n                \"type\": \"integer\",\n                \"description\": \"Number of days after creation that a recovery point is moved to cold storage.\"\
  \n              },\n              \"deleteAfterDays\": {\n                \"type\": \"integer\",\n                \"description\": \"Number of days after creation that a recovery point is deleted.\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"advancedBackupSettings\": {\n      \"type\": \"array\",\n      \"description\": \"Advanced backup settings for the backup plan.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"resourceType\": {\n            \"type\": \"string\",\n            \"description\": \"The type of AWS resource to be backed up.\"\n          },\n          \"backupOptions\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-backup/refs/heads/main/json-schema/amazon-backup-plan-schema.json
tags:
- AWS
- Backup
- Data Protection
- Disaster Recovery
- Storage
- Compliance
- Governance
- Business Continuity
title: Amazon Backup Plan
---
