---
description: Represents a flow configuration for the Lunar Gateway. Flows are YAML-based definitions that describe how API requests and responses are processed in real time, including traffic management rules such as rate limiting, caching, retry mechanisms, quota enforcement, and request prioritization.
layout: schema
name: Lunar.dev Flow
properties_list:
- description: Human-readable name for the flow.
  name: name
  type: string
- description: Description of the flow and its purpose.
  name: description
  type: string
- description: Whether the flow is currently active.
  name: enabled
  type: boolean
- description: Filter criteria that determine which requests this flow applies to.
  name: filter
  type: object
- description: Ordered list of processors to apply to matched requests.
  name: processors
  type: array
provider_name: Lunar.dev
provider_slug: lunar-dev
schema_file: json-schema/flow.json
slug: flow
source_filename: flow.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/lunar-dev/blob/main/json-schema/flow.json\",\n  \"title\": \"Lunar.dev Flow\",\n  \"description\": \"Represents a flow configuration for the Lunar Gateway. Flows are YAML-based definitions that describe how API requests and responses are processed in real time, including traffic management rules such as rate limiting, caching, retry mechanisms, quota enforcement, and request prioritization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the flow.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the flow and its purpose.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the flow is currently active.\",\n      \"default\": true\n    },\n    \"filter\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"Filter criteria that determine which requests this flow applies to.\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"description\": \"URL pattern to match against incoming requests.\"\n        },\n        \"method\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP method to match.\"\n        },\n        \"headers\": {\n          \"type\": \"object\",\n          \"description\": \"Header key-value pairs to match.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"processors\": {\n      \"type\": \"array\",\n      \"description\": \"Ordered list of processors to apply to matched requests.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The processor type.\",\n            \"examples\": [\n \
  \             \"rate_limit\",\n              \"cache\",\n              \"retry\",\n              \"queue\",\n              \"quota\"\n            ]\n          },\n          \"config\": {\n            \"type\": \"object\",\n            \"description\": \"Processor-specific configuration parameters.\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lunar-dev/refs/heads/main/json-schema/flow.json
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
title: Lunar.dev Flow
---
