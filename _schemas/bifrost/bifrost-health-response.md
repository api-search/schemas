---
description: Gateway health status response.
layout: schema
name: HealthResponse
properties_list:
- description: Overall gateway status.
  name: status
  type: string
- description: Gateway version.
  name: version
  type: string
- description: Status of configured providers.
  name: providers
  type: array
provider_name: Bifrost
provider_slug: bifrost
schema_file: json-schema/bifrost-health-response-schema.json
slug: bifrost-health-response
source_filename: bifrost-health-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HealthResponse\",\n  \"type\": \"object\",\n  \"description\": \"Gateway health status response.\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Overall gateway status.\",\n      \"example\": \"ok\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Gateway version.\",\n      \"example\": \"v1.0.0\"\n    },\n    \"providers\": {\n      \"type\": \"array\",\n      \"description\": \"Status of configured providers.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ProviderStatus\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bifrost/refs/heads/main/json-schema/bifrost-health-response-schema.json
tags:
- AI Gateway
- LLM
- Load Balancing
- Open Source
- OpenAI Compatible
- MCP
title: HealthResponse
---
