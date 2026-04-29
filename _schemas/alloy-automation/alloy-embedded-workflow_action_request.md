---
description: Request body for workflow lifecycle actions
layout: schema
name: WorkflowActionRequest
properties_list:
- description: Unique identifier of the workflow
  name: workflowId
  type: string
- description: Identifier of the user
  name: userId
  type: string
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-embedded-workflow_action_request-schema.json
slug: alloy-embedded-workflow_action_request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-embedded-workflow_action_request-schema.json\",\n  \"title\": \"WorkflowActionRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for workflow lifecycle actions\",\n  \"properties\": {\n    \"workflowId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the workflow\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the user\"\n    }\n  },\n  \"required\": [\n    \"workflowId\",\n    \"userId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-embedded-workflow_action_request-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: WorkflowActionRequest
---
