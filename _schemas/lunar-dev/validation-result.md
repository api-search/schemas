---
description: Represents the result of validating a policy or flow configuration against the Lunar Gateway. Indicates whether the configuration is valid and lists any errors found.
layout: schema
name: Lunar.dev Validation Result
properties_list:
- description: Whether the configuration is valid.
  name: valid
  type: boolean
- description: List of validation errors found, if any.
  name: errors
  type: array
provider_name: Lunar.dev
provider_slug: lunar-dev
schema_file: json-schema/validation-result.json
slug: validation-result
source_filename: validation-result.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/lunar-dev/blob/main/json-schema/validation-result.json\",\n  \"title\": \"Lunar.dev Validation Result\",\n  \"description\": \"Represents the result of validating a policy or flow configuration against the Lunar Gateway. Indicates whether the configuration is valid and lists any errors found.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"valid\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the configuration is valid.\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of validation errors found, if any.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lunar-dev/refs/heads/main/json-schema/validation-result.json
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
title: Lunar.dev Validation Result
---
