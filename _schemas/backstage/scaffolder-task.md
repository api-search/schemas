---
description: Task schema from Backstage scaffolder API
layout: schema
name: Task
properties_list:
- description: The unique identifier of the task.
  name: id
  type: string
- description: ''
  name: spec
  type: object
- description: The current status of the task.
  name: status
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: lastHeartbeatAt
  type: string
- description: ''
  name: completedAt
  type: string
- description: The user who created the task.
  name: createdBy
  type: string
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/scaffolder-task-schema.json
slug: scaffolder-task
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/scaffolder-task-schema.json\",\n  \"title\": \"Task\",\n  \"description\": \"Task schema from Backstage scaffolder API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the task.\"\n    },\n    \"spec\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"apiVersion\": {\n          \"type\": \"string\"\n        },\n        \"templateInfo\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"entityRef\": {\n              \"type\": \"string\",\n              \"description\": \"Reference to the template entity.\"\n            }\n          }\n        },\n        \"steps\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n           \
  \ \"properties\": {\n              \"id\": {\n                \"type\": \"string\"\n              },\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"action\": {\n                \"type\": \"string\"\n              },\n              \"input\": {\n                \"type\": \"object\"\n              }\n            }\n          }\n        },\n        \"output\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        },\n        \"parameters\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the task.\",\n      \"enum\": [\n        \"open\",\n        \"processing\",\n        \"completed\",\n        \"failed\",\n        \"cancelled\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"lastHeartbeatAt\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"The user who created the task.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/scaffolder-task-schema.json
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: Task
---
