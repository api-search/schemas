---
description: List of workflow execution logs
layout: schema
name: WorkflowLogList
properties_list:
- description: List of log entries
  name: logs
  type: array
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-embedded-workflow_log_list-schema.json
slug: alloy-embedded-workflow_log_list
source_filename: alloy-embedded-workflow_log_list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-embedded-workflow_log_list-schema.json\",\n  \"title\": \"WorkflowLogList\",\n  \"type\": \"object\",\n  \"description\": \"List of workflow execution logs\",\n  \"properties\": {\n    \"logs\": {\n      \"type\": \"array\",\n      \"description\": \"List of log entries\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-embedded-workflow_log_list-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: WorkflowLogList
---
