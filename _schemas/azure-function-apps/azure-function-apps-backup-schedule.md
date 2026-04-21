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
provider_name: Azure Function Apps
provider_slug: azure-function-apps
schema_file: json-schema/azure-function-apps-backup-schedule-schema.json
slug: azure-function-apps-backup-schedule
tags:
- Azure
- Compute
- FaaS
- Functions
- Serverless
title: BackupSchedule
---
