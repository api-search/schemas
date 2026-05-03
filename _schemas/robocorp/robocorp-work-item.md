---
description: Schema for a Robocorp Control Room work item used in RPA process queues.
layout: schema
name: Robocorp Work Item
properties_list:
- description: Unique work item identifier
  name: id
  type: string
- description: Identifier of the process this work item belongs to
  name: process_id
  type: string
- description: Current state of the work item
  name: state
  type: string
- description: Arbitrary input data payload for the work item
  name: payload
  type: object
- description: Timestamp when the work item was created
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: Error details if the work item failed
  name: exception
  type: object
provider_name: Robocorp
provider_slug: robocorp
schema_file: json-schema/robocorp-work-item-schema.json
slug: robocorp-work-item
source_filename: robocorp-work-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/robocorp/json-schema/robocorp-work-item-schema.json\",\n  \"title\": \"Robocorp Work Item\",\n  \"description\": \"Schema for a Robocorp Control Room work item used in RPA process queues.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique work item identifier\"\n    },\n    \"process_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the process this work item belongs to\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current state of the work item\",\n      \"enum\": [\"PENDING\", \"INPROGRESS\", \"COMPLETED\", \"FAILED\"]\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"description\": \"Arbitrary input data payload for the work item\",\n      \"additionalProperties\": true\n    },\n    \"created_at\": {\n      \"\
  type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the work item was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"exception\": {\n      \"type\": \"object\",\n      \"description\": \"Error details if the work item failed\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Exception type\"\n        },\n        \"code\": {\n          \"type\": \"string\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Error message\"\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"process_id\", \"state\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/json-schema/robocorp-work-item-schema.json
tags:
- RPA
- Workflow Automation
- Python
- Open Source
- Automation
title: Robocorp Work Item
---
