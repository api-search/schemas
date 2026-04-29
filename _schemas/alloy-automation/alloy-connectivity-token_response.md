---
description: JWT token response
layout: schema
name: TokenResponse
properties_list:
- description: Short-lived JSON Web Token
  name: token
  type: string
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-connectivity-token_response-schema.json
slug: alloy-connectivity-token_response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-connectivity-token_response-schema.json\",\n  \"title\": \"TokenResponse\",\n  \"type\": \"object\",\n  \"description\": \"JWT token response\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"Short-lived JSON Web Token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-connectivity-token_response-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: TokenResponse
---
