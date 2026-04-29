---
description: Represents a backup job in Commvault, tracking the execution of a data protection operation including its status, progress, data transfer metrics, and associated client and subclient information.
layout: schema
name: Commvault Backup Job
properties_list:
- description: Unique identifier for the backup job
  name: jobId
  type: integer
- description: Type of job operation
  name: jobType
  type: string
- description: Current status of the job
  name: status
  type: string
- description: Backup level for backup jobs
  name: backupLevel
  type: string
- description: The subclient associated with this job
  name: subclient
  type: object
- description: Job completion percentage
  name: percentComplete
  type: integer
- description: Timestamp when the job started
  name: startTime
  type: string
- description: Timestamp when the job completed
  name: endTime
  type: string
- description: Total elapsed time of the job in seconds
  name: elapsedTimeSeconds
  type: integer
- description: Total size of application data processed in bytes
  name: sizeOfBackupBytes
  type: integer
- description: Total size of data written to storage media in bytes
  name: sizeOfMediaOnDiskBytes
  type: integer
- description: Number of files processed during the job
  name: numOfFiles
  type: integer
- description: Reason for job failure if the job did not complete successfully
  name: failureReason
  type: string
- description: Name of the storage policy used for data placement
  name: storagePolicyName
  type: string
- description: Name of the media agent that processed the job
  name: mediaAgent
  type: string
- description: Whether the job data has been aged out (pruned by retention policy)
  name: isAged
  type: boolean
provider_name: Commvault
provider_slug: commvault
schema_file: json-schema/commvault-backup-job-schema.json
slug: commvault-backup-job
source_filename: commvault-backup-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.commvault.com/schemas/commvault/backup-job.json\",\n  \"title\": \"Commvault Backup Job\",\n  \"description\": \"Represents a backup job in Commvault, tracking the execution of a data protection operation including its status, progress, data transfer metrics, and associated client and subclient information.\",\n  \"type\": \"object\",\n  \"required\": [\"jobId\", \"jobType\", \"status\"],\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the backup job\"\n    },\n    \"jobType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of job operation\",\n      \"enum\": [\"Backup\", \"Restore\", \"Auxiliary Copy\", \"Data Aging\", \"Synthetic Full\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the job\",\n      \"enum\": [\n        \"Running\",\n       \
  \ \"Waiting\",\n        \"Pending\",\n        \"Completed\",\n        \"Completed w/ one or more errors\",\n        \"Completed w/ one or more warnings\",\n        \"Failed\",\n        \"Killed\",\n        \"Suspended\"\n      ]\n    },\n    \"backupLevel\": {\n      \"type\": \"string\",\n      \"description\": \"Backup level for backup jobs\",\n      \"enum\": [\"Full\", \"Incremental\", \"Differential\", \"Synthetic Full\", \"Transaction Log\"]\n    },\n    \"subclient\": {\n      \"type\": \"object\",\n      \"description\": \"The subclient associated with this job\",\n      \"properties\": {\n        \"subclientId\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique subclient identifier\"\n        },\n        \"subclientName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the subclient\"\n        },\n        \"clientName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the parent client\"\n        },\n \
  \       \"appName\": {\n          \"type\": \"string\",\n          \"description\": \"Agent or application name\"\n        }\n      }\n    },\n    \"percentComplete\": {\n      \"type\": \"integer\",\n      \"description\": \"Job completion percentage\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the job started\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the job completed\"\n    },\n    \"elapsedTimeSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Total elapsed time of the job in seconds\",\n      \"minimum\": 0\n    },\n    \"sizeOfBackupBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Total size of application data processed in bytes\",\n      \"minimum\": 0\n    },\n    \"sizeOfMediaOnDiskBytes\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Total size of data written to storage media in bytes\",\n      \"minimum\": 0\n    },\n    \"numOfFiles\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of files processed during the job\",\n      \"minimum\": 0\n    },\n    \"failureReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for job failure if the job did not complete successfully\"\n    },\n    \"storagePolicyName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the storage policy used for data placement\"\n    },\n    \"mediaAgent\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the media agent that processed the job\"\n    },\n    \"isAged\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the job data has been aged out (pruned by retention policy)\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/commvault/refs/heads/main/json-schema/commvault-backup-job-schema.json
tags:
- Backup
- Cloud Storage
- Cyber Recovery
- Data Management
- Data Protection
- Disaster Recovery
- Enterprise Software
title: Commvault Backup Job
---
