---
description: Standard error response
layout: schema
name: ErrorResponse
properties_list:
- description: Error code or type
  name: error
  type: string
- description: Human-readable error description
  name: message
  type: string
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-connectivity-error_response-schema.json
slug: alloy-connectivity-error_response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-connectivity-error_response-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Standard error response\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error code or type\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error description\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-connectivity-error_response-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: ErrorResponse
---
