---
description: Response from triggering a workflow execution.
layout: schema
name: WorkflowRunResponse
properties_list:
- description: ''
  name: data
  type: object
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-workflow-run-response-schema.json
slug: bettercloud-workflow-run-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-workflow-run-response-schema.json\",\n  \"title\": \"WorkflowRunResponse\",\n  \"description\": \"Response from triggering a workflow execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"execution_id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique ID of this workflow execution.\",\n          \"example\": \"exec-900100\"\n        },\n        \"workflow_id\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the workflow being executed.\",\n          \"example\": \"wf-100200\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Current execution status.\",\n          \"enum\": [\n            \"pending\",\n          \
  \  \"running\",\n            \"completed\",\n            \"failed\"\n          ],\n          \"example\": \"running\"\n        },\n        \"started_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the execution started.\",\n          \"example\": \"2026-04-19T10:00:00Z\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-workflow-run-response-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: WorkflowRunResponse
---
