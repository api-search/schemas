---
description: Attributes of a NetBackup job
layout: schema
name: JobAttributes
properties_list:
- description: Unique identifier for the job
  name: jobId
  type: integer
- description: Identifier of the parent job, if this is a child job
  name: parentJobId
  type: integer
- description: The type of job
  name: jobType
  type: string
- description: Current state of the job
  name: state
  type: string
- description: Exit status code of the job. A value of 0 indicates success.
  name: status
  type: integer
- description: Name of the policy associated with the job
  name: policyName
  type: string
- description: Type of the policy (e.g., Standard, VMware, Oracle)
  name: policyType
  type: string
- description: Name of the schedule that triggered the job
  name: scheduleName
  type: string
- description: Type of the schedule
  name: scheduleType
  type: string
- description: Hostname of the client being backed up or restored
  name: clientName
  type: string
- description: Hostname of the media server processing the job
  name: mediaServer
  type: string
- description: Name of the storage unit used by the job
  name: storageUnit
  type: string
- description: Timestamp when the job started
  name: startTime
  type: string
- description: Timestamp when the job completed or was last updated
  name: endTime
  type: string
- description: Total elapsed time in seconds
  name: elapsedTime
  type: integer
- description: Total kilobytes of data transferred
  name: kilobytesTransferred
  type: integer
- description: Total number of files processed
  name: filesTransferred
  type: integer
- description: Completion percentage (0-100)
  name: percentComplete
  type: integer
- description: Description of the operation currently being performed
  name: currentOperation
  type: string
- description: Current attempt number for the job
  name: attempt
  type: integer
- description: Whether the job can be restarted
  name: restartable
  type: boolean
- description: Whether the job can be suspended
  name: suspendable
  type: boolean
- description: Whether the job can be resumed
  name: resumable
  type: boolean
- description: Whether the job can be cancelled
  name: cancellable
  type: boolean
provider_name: Veritas NetBackup
provider_slug: veritas-netbackup
schema_file: json-schema/veritas-netbackup-rest-job-attributes-schema.json
slug: veritas-netbackup-rest-job-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobAttributes\",\n  \"type\": \"object\",\n  \"description\": \"Attributes of a NetBackup job\",\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the job\"\n    },\n    \"parentJobId\": {\n      \"type\": \"integer\",\n      \"description\": \"Identifier of the parent job, if this is a child job\"\n    },\n    \"jobType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of job\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current state of the job\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"Exit status code of the job. A value of 0 indicates success.\"\n    },\n    \"policyName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the policy associated with the job\"\n    },\n    \"policyType\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Type of the policy (e.g., Standard, VMware, Oracle)\"\n    },\n    \"scheduleName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the schedule that triggered the job\"\n    },\n    \"scheduleType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the schedule\"\n    },\n    \"clientName\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the client being backed up or restored\"\n    },\n    \"mediaServer\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the media server processing the job\"\n    },\n    \"storageUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the storage unit used by the job\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the job started\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the job completed or was last updated\"\n \
  \   },\n    \"elapsedTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Total elapsed time in seconds\"\n    },\n    \"kilobytesTransferred\": {\n      \"type\": \"integer\",\n      \"description\": \"Total kilobytes of data transferred\"\n    },\n    \"filesTransferred\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of files processed\"\n    },\n    \"percentComplete\": {\n      \"type\": \"integer\",\n      \"description\": \"Completion percentage (0-100)\"\n    },\n    \"currentOperation\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the operation currently being performed\"\n    },\n    \"attempt\": {\n      \"type\": \"integer\",\n      \"description\": \"Current attempt number for the job\"\n    },\n    \"restartable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the job can be restarted\"\n    },\n    \"suspendable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the job\
  \ can be suspended\"\n    },\n    \"resumable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the job can be resumed\"\n    },\n    \"cancellable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the job can be cancelled\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/veritas-netbackup/refs/heads/main/json-schema/veritas-netbackup-rest-job-attributes-schema.json
tags:
- Backup
- Data Protection
- Disaster Recovery
- Enterprise
- Recovery
- Storage
title: JobAttributes
---
