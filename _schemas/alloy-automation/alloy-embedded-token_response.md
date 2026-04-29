---
description: JWT token response for user authentication
layout: schema
name: TokenResponse
properties_list:
- description: Short-lived JSON Web Token for frontend SDK authentication
  name: token
  type: string
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-embedded-token_response-schema.json
slug: alloy-embedded-token_response
source_filename: alloy-embedded-token_response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-embedded-token_response-schema.json\",\n  \"title\": \"TokenResponse\",\n  \"type\": \"object\",\n  \"description\": \"JWT token response for user authentication\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"Short-lived JSON Web Token for frontend SDK authentication\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-embedded-token_response-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: TokenResponse
---
