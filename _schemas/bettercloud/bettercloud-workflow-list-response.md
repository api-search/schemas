---
description: Paginated list of workflows.
layout: schema
name: WorkflowListResponse
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: meta
  type: object
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-workflow-list-response-schema.json
slug: bettercloud-workflow-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-workflow-list-response-schema.json\",\n  \"title\": \"WorkflowListResponse\",\n  \"description\": \"Paginated list of workflows.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Workflow\"\n      }\n    },\n    \"meta\": {\n      \"$ref\": \"#/components/schemas/MetaResponse\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-workflow-list-response-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: WorkflowListResponse
---
