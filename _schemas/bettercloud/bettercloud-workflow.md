---
description: An automation workflow that can be triggered to execute actions across SaaS applications.
layout: schema
name: Workflow
properties_list:
- description: Unique identifier of the workflow.
  name: id
  type: string
- description: Display name of the workflow.
  name: name
  type: string
- description: Description of what the workflow does.
  name: description
  type: string
- description: Current status of the workflow.
  name: status
  type: string
- description: How the workflow is triggered.
  name: trigger_type
  type: string
- description: Number of actions in the workflow.
  name: action_count
  type: integer
- description: When the workflow was created.
  name: created_at
  type: string
- description: When the workflow was last updated.
  name: updated_at
  type: string
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-workflow-schema.json
slug: bettercloud-workflow
source_filename: bettercloud-workflow-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-workflow-schema.json\",\n  \"title\": \"Workflow\",\n  \"description\": \"An automation workflow that can be triggered to execute actions across SaaS applications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the workflow.\",\n      \"example\": \"wf-100200\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the workflow.\",\n      \"example\": \"Employee Offboarding\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Description of what the workflow does.\",\n      \"example\": \"Automated offboarding workflow for departing employees\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Current status of the workflow.\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"draft\"\n      ],\n      \"example\": \"active\"\n    },\n    \"trigger_type\": {\n      \"type\": \"string\",\n      \"description\": \"How the workflow is triggered.\",\n      \"enum\": [\n        \"manual\",\n        \"event\",\n        \"scheduled\"\n      ],\n      \"example\": \"manual\"\n    },\n    \"action_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of actions in the workflow.\",\n      \"example\": 12\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the workflow was created.\",\n      \"example\": \"2025-03-01T00:00:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"When the workflow was last updated.\",\n      \"example\": \"2026-04-01T00:00:00Z\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-workflow-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: Workflow
---
