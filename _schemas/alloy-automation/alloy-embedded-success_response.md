---
description: Standard success response
layout: schema
name: SuccessResponse
properties_list:
- description: Whether the operation succeeded
  name: success
  type: boolean
- description: Human-readable success message
  name: message
  type: string
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-embedded-success_response-schema.json
slug: alloy-embedded-success_response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-embedded-success_response-schema.json\",\n  \"title\": \"SuccessResponse\",\n  \"type\": \"object\",\n  \"description\": \"Standard success response\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the operation succeeded\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable success message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-embedded-success_response-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: SuccessResponse
---
