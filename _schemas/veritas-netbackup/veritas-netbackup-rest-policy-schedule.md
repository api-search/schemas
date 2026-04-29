---
description: ''
layout: schema
name: PolicySchedule
properties_list:
- description: Name of the schedule
  name: scheduleName
  type: string
- description: Type of backup for this schedule
  name: scheduleType
  type: string
- description: Frequency in seconds between backup runs
  name: frequency
  type: integer
- description: ''
  name: retentionPeriod
  type: object
- description: Name of the storage unit for this schedule
  name: storageUnit
  type: string
- description: ''
  name: backupWindow
  type: object
- description: Maximum number of concurrent backup streams to a single device
  name: mediaMultiplexing
  type: integer
- description: Whether this schedule creates synthetic backups
  name: syntheticBackup
  type: boolean
provider_name: Veritas NetBackup
provider_slug: veritas-netbackup
schema_file: json-schema/veritas-netbackup-rest-policy-schedule-schema.json
slug: veritas-netbackup-rest-policy-schedule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PolicySchedule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scheduleName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the schedule\"\n    },\n    \"scheduleType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of backup for this schedule\"\n    },\n    \"frequency\": {\n      \"type\": \"integer\",\n      \"description\": \"Frequency in seconds between backup runs\"\n    },\n    \"retentionPeriod\": {\n      \"type\": \"object\"\n    },\n    \"storageUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the storage unit for this schedule\"\n    },\n    \"backupWindow\": {\n      \"type\": \"object\"\n    },\n    \"mediaMultiplexing\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of concurrent backup streams to a single device\"\n    },\n    \"syntheticBackup\": {\n      \"type\": \"boolean\",\n \
  \     \"description\": \"Whether this schedule creates synthetic backups\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/veritas-netbackup/refs/heads/main/json-schema/veritas-netbackup-rest-policy-schedule-schema.json
tags:
- Backup
- Data Protection
- Disaster Recovery
- Enterprise
- Recovery
- Storage
title: PolicySchedule
---
