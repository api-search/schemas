---
description: Schema for a Robocorp Control Room automation process definition.
layout: schema
name: Robocorp Process
properties_list:
- description: Unique process identifier
  name: id
  type: string
- description: Human-readable process name
  name: name
  type: string
- description: Description of what this process automates
  name: description
  type: string
- description: Current state of the process
  name: state
  type: string
- description: Ordered list of process execution steps
  name: steps
  type: array
- description: Scheduled triggers for automatic execution
  name: schedules
  type: array
- description: ''
  name: created_at
  type: string
provider_name: Robocorp
provider_slug: robocorp
schema_file: json-schema/robocorp-process-schema.json
slug: robocorp-process
source_filename: robocorp-process-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/robocorp/json-schema/robocorp-process-schema.json\",\n  \"title\": \"Robocorp Process\",\n  \"description\": \"Schema for a Robocorp Control Room automation process definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique process identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable process name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what this process automates\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current state of the process\",\n      \"enum\": [\"active\", \"disabled\"]\n    },\n    \"steps\": {\n      \"type\": \"array\",\n      \"description\": \"Ordered list of process execution steps\",\n      \"items\": {\n        \"\
  type\": \"object\",\n        \"properties\": {\n          \"name\": { \"type\": \"string\" },\n          \"package_id\": {\n            \"type\": \"string\",\n            \"description\": \"Task package ID for this step\"\n          },\n          \"worker_group_id\": {\n            \"type\": \"string\",\n            \"description\": \"Worker group to run this step\"\n          }\n        }\n      }\n    },\n    \"schedules\": {\n      \"type\": \"array\",\n      \"description\": \"Scheduled triggers for automatic execution\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"cron\": {\n            \"type\": \"string\",\n            \"description\": \"Cron expression for scheduling\"\n          },\n          \"timezone\": {\n            \"type\": \"string\",\n            \"description\": \"Timezone for the schedule\"\n          },\n          \"enabled\": {\n            \"type\": \"boolean\"\n          }\n        }\n      }\n    },\n    \"created_at\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/json-schema/robocorp-process-schema.json
tags:
- RPA
- Workflow Automation
- Python
- Open Source
- Automation
title: Robocorp Process
---
