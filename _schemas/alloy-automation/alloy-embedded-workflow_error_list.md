---
description: List of workflow execution errors
layout: schema
name: WorkflowErrorList
properties_list:
- description: List of error records
  name: errors
  type: array
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-embedded-workflow_error_list-schema.json
slug: alloy-embedded-workflow_error_list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-embedded-workflow_error_list-schema.json\",\n  \"title\": \"WorkflowErrorList\",\n  \"type\": \"object\",\n  \"description\": \"List of workflow execution errors\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of error records\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-embedded-workflow_error_list-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: WorkflowErrorList
---
