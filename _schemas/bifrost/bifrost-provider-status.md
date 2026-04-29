---
description: Status of a configured AI provider.
layout: schema
name: ProviderStatus
properties_list:
- description: Provider name.
  name: name
  type: string
- description: Provider health status.
  name: status
  type: string
provider_name: Bifrost
provider_slug: bifrost
schema_file: json-schema/bifrost-provider-status-schema.json
slug: bifrost-provider-status
source_filename: bifrost-provider-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ProviderStatus\",\n  \"type\": \"object\",\n  \"description\": \"Status of a configured AI provider.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Provider name.\",\n      \"example\": \"openai\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Provider health status.\",\n      \"enum\": [\n        \"healthy\",\n        \"degraded\",\n        \"unavailable\"\n      ],\n      \"example\": \"healthy\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bifrost/refs/heads/main/json-schema/bifrost-provider-status-schema.json
tags:
- AI Gateway
- LLM
- Load Balancing
- Open Source
- OpenAI Compatible
- MCP
title: ProviderStatus
---
