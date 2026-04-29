---
description: Metadata about the API response.
layout: schema
name: ResponseMetadata
properties_list:
- description: Unique identifier for this API request.
  name: request_id
  type: string
- description: Time taken to complete the request in milliseconds.
  name: response_time_ms
  type: integer
provider_name: AgentQL
provider_slug: agentql
schema_file: json-schema/agentql-response-metadata-schema.json
slug: agentql-response-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/json-schema/agentql-response-metadata-schema.json\",\n  \"title\": \"ResponseMetadata\",\n  \"description\": \"Metadata about the API response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this API request.\",\n      \"example\": \"req-a1b2c3d4\"\n    },\n    \"response_time_ms\": {\n      \"type\": \"integer\",\n      \"description\": \"Time taken to complete the request in milliseconds.\",\n      \"example\": 1847\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/json-schema/agentql-response-metadata-schema.json
tags:
- Agents
- Artificial Intelligence
- Web Scraping
- Data Extraction
- Browser Automation
- REST API
title: ResponseMetadata
---
