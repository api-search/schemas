---
description: Detailed representation of a schedule
layout: schema
name: ScheduleDetail
properties_list:
- description: Unique schedule identifier
  name: id
  type: string
- description: Name of the schedule
  name: name
  type: string
- description: ID of the associated workflow
  name: workflowId
  type: string
- description: Specific workflow version ID
  name: versionId
  type: string
- description: ID of the schedule owner
  name: ownerId
  type: string
- description: Next scheduled run date and time
  name: runDateTime
  type: string
- description: Comments about the schedule
  name: comment
  type: string
- description: Whether the schedule is active
  name: enabled
  type: boolean
- description: Execution priority
  name: priority
  type: string
- description: Worker tag for execution routing
  name: workerTag
  type: string
- description: Current status of the schedule
  name: status
  type: string
- description: Credential used for execution
  name: credentialId
  type: string
- description: When the schedule was created
  name: creationTime
  type: string
- description: When the schedule last executed
  name: lastRunTime
  type: string
- description: Current state of the schedule
  name: state
  type: string
- description: Total number of times the schedule has executed
  name: runCount
  type: integer
- description: Human-readable frequency description
  name: frequency
  type: string
- description: Last error message if any
  name: lastError
  type: string
- description: Name of the worker node
  name: cpuName
  type: string
- description: ID of the user who last modified the schedule
  name: lastModifiedId
  type: string
- description: Date of last modification
  name: lastModifiedDate
  type: string
- description: Whether the current user can edit this schedule
  name: canEdit
  type: boolean
- description: Time zone for the schedule
  name: timeZone
  type: string
- description: Analytic app question values
  name: questions
  type: array
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-schedule-detail-schema.json
slug: alteryx-server-v3-schedule-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScheduleDetail\",\n  \"type\": \"object\",\n  \"description\": \"Detailed representation of a schedule\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique schedule identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the schedule\"\n    },\n    \"workflowId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the associated workflow\"\n    },\n    \"versionId\": {\n      \"type\": \"string\",\n      \"description\": \"Specific workflow version ID\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the schedule owner\"\n    },\n    \"runDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Next scheduled run date and time\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Comments about the schedule\"\
  \n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the schedule is active\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"Execution priority\"\n    },\n    \"workerTag\": {\n      \"type\": \"string\",\n      \"description\": \"Worker tag for execution routing\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the schedule\"\n    },\n    \"credentialId\": {\n      \"type\": \"string\",\n      \"description\": \"Credential used for execution\"\n    },\n    \"creationTime\": {\n      \"type\": \"string\",\n      \"description\": \"When the schedule was created\"\n    },\n    \"lastRunTime\": {\n      \"type\": \"string\",\n      \"description\": \"When the schedule last executed\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current state of the schedule\"\n    },\n    \"runCount\": {\n      \"type\": \"integer\",\n      \"\
  description\": \"Total number of times the schedule has executed\"\n    },\n    \"frequency\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable frequency description\"\n    },\n    \"lastError\": {\n      \"type\": \"string\",\n      \"description\": \"Last error message if any\"\n    },\n    \"cpuName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the worker node\"\n    },\n    \"lastModifiedId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who last modified the schedule\"\n    },\n    \"lastModifiedDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of last modification\"\n    },\n    \"canEdit\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the current user can edit this schedule\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\",\n      \"description\": \"Time zone for the schedule\"\n    },\n    \"questions\": {\n      \"type\": \"array\",\n      \"description\":\
  \ \"Analytic app question values\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-schedule-detail-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: ScheduleDetail
---
