---
description: Worker queue metrics
layout: schema
name: QueueMetrics
properties_list:
- description: ''
  name: queues
  type: array
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-queue-metrics-schema.json
slug: activepieces-queue-metrics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-queue-metrics-schema.json\",\n  \"title\": \"QueueMetrics\",\n  \"description\": \"Worker queue metrics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queues\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Queue name\",\n            \"example\": \"one-time\"\n          },\n          \"waiting\": {\n            \"type\": \"integer\",\n            \"description\": \"Jobs waiting\",\n            \"example\": 5\n          },\n          \"active\": {\n            \"type\": \"integer\",\n            \"description\": \"Jobs active\",\n            \"example\": 2\n          },\n          \"completed\": {\n            \"type\": \"integer\",\n\
  \            \"description\": \"Jobs completed\",\n            \"example\": 1000\n          },\n          \"failed\": {\n            \"type\": \"integer\",\n            \"description\": \"Jobs failed\",\n            \"example\": 3\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-queue-metrics-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: QueueMetrics
---
