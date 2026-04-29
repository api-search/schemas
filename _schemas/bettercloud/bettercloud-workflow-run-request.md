---
description: Request body for triggering a workflow execution.
layout: schema
name: WorkflowRunRequest
properties_list:
- description: List of user IDs to run the workflow for.
  name: user_ids
  type: array
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-workflow-run-request-schema.json
slug: bettercloud-workflow-run-request
source_filename: bettercloud-workflow-run-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-workflow-run-request-schema.json\",\n  \"title\": \"WorkflowRunRequest\",\n  \"description\": \"Request body for triggering a workflow execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"user_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of user IDs to run the workflow for.\",\n      \"example\": [\n        \"user-a1b2c3d4\"\n      ]\n    }\n  },\n  \"required\": [\n    \"user_ids\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-workflow-run-request-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: WorkflowRunRequest
---
