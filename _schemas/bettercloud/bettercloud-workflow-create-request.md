---
description: Request body for creating a workflow.
layout: schema
name: WorkflowCreateRequest
properties_list:
- description: Name of the workflow.
  name: name
  type: string
- description: Description of the workflow.
  name: description
  type: string
- description: Trigger type for the workflow.
  name: trigger_type
  type: string
- description: Initial status.
  name: status
  type: string
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-workflow-create-request-schema.json
slug: bettercloud-workflow-create-request
source_filename: bettercloud-workflow-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-workflow-create-request-schema.json\",\n  \"title\": \"WorkflowCreateRequest\",\n  \"description\": \"Request body for creating a workflow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the workflow.\",\n      \"example\": \"New Employee Onboarding\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the workflow.\",\n      \"example\": \"Automated onboarding workflow for new hires\"\n    },\n    \"trigger_type\": {\n      \"type\": \"string\",\n      \"description\": \"Trigger type for the workflow.\",\n      \"enum\": [\n        \"manual\",\n        \"event\",\n        \"scheduled\"\n      ],\n      \"example\": \"event\"\n    },\n    \"status\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Initial status.\",\n      \"enum\": [\n        \"active\",\n        \"draft\"\n      ],\n      \"example\": \"draft\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-workflow-create-request-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: WorkflowCreateRequest
---
