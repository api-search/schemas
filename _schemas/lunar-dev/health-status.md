---
description: Represents the health status of a running Lunar Gateway instance, indicating whether the gateway is healthy and ready to process traffic.
layout: schema
name: Lunar.dev Health Status
properties_list:
- description: The health status of the gateway.
  name: status
  type: string
provider_name: Lunar.dev
provider_slug: lunar-dev
schema_file: json-schema/health-status.json
slug: health-status
source_filename: health-status.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/lunar-dev/blob/main/json-schema/health-status.json\",\n  \"title\": \"Lunar.dev Health Status\",\n  \"description\": \"Represents the health status of a running Lunar Gateway instance, indicating whether the gateway is healthy and ready to process traffic.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The health status of the gateway.\",\n      \"examples\": [\n        \"healthy\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lunar-dev/refs/heads/main/json-schema/health-status.json
tags:
- AI Gateway
- Automation
- Consumption Gateway
- Control
- Deployment
- Integrations
- MCP Gateway
- Performance
- Platform
- Version Control
- Visibility
- Workflows
title: Lunar.dev Health Status
---
