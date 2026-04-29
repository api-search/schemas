---
description: Cache control settings for prompt caching.
layout: schema
name: CacheControl
properties_list:
- description: ''
  name: type
  type: string
- description: Time-to-live for the cache entry.
  name: ttl
  type: string
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-cache-control-schema.json
slug: claude-messages-cache-control
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CacheControl\",\n  \"type\": \"object\",\n  \"description\": \"Cache control settings for prompt caching.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"ttl\": {\n      \"type\": \"string\",\n      \"description\": \"Time-to-live for the cache entry.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-cache-control-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: CacheControl
---
