---
description: Represents a policy configuration for the Lunar Gateway. Policies define rules for traffic management including rate limiting, quota enforcement, caching, and other controls applied to API requests passing through the gateway.
layout: schema
name: Lunar.dev Policy
properties_list:
- description: Human-readable name for the policy.
  name: name
  type: string
- description: Description of the policy and its purpose.
  name: description
  type: string
- description: Whether the policy is currently active.
  name: enabled
  type: boolean
- description: The target endpoint pattern this policy applies to.
  name: endpoint
  type: string
- description: HTTP method this policy applies to. If omitted, applies to all methods.
  name: method
  type: string
- description: The type of policy to enforce.
  name: type
  type: string
- description: Policy-specific configuration parameters.
  name: config
  type: object
- description: Optional consumer tag to scope the policy to a specific consumer.
  name: consumer_tag
  type: string
provider_name: Lunar.dev
provider_slug: lunar-dev
schema_file: json-schema/policy.json
slug: policy
source_filename: policy.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/lunar-dev/blob/main/json-schema/policy.json\",\n  \"title\": \"Lunar.dev Policy\",\n  \"description\": \"Represents a policy configuration for the Lunar Gateway. Policies define rules for traffic management including rate limiting, quota enforcement, caching, and other controls applied to API requests passing through the gateway.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the policy.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the policy and its purpose.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the policy is currently active.\",\n      \"default\": true\n    },\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The target endpoint\
  \ pattern this policy applies to.\",\n      \"examples\": [\n        \"api.example.com/v1/*\"\n      ]\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"description\": \"HTTP method this policy applies to. If omitted, applies to all methods.\",\n      \"examples\": [\n        \"GET\",\n        \"POST\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of policy to enforce.\",\n      \"examples\": [\n        \"rate_limit\",\n        \"quota\",\n        \"caching\",\n        \"retry\"\n      ]\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"description\": \"Policy-specific configuration parameters.\"\n    },\n    \"consumer_tag\": {\n      \"type\": \"string\",\n      \"description\": \"Optional consumer tag to scope the policy to a specific consumer.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lunar-dev/refs/heads/main/json-schema/policy.json
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
title: Lunar.dev Policy
---
