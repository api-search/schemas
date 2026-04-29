---
description: Request metadata for tracking and abuse prevention.
layout: schema
name: Metadata
properties_list:
- description: An external identifier for the user making the request. Should be a UUID, hash, or other opaque identifier.
  name: user_id
  type: string
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-metadata-schema.json
slug: claude-messages-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Metadata\",\n  \"type\": \"object\",\n  \"description\": \"Request metadata for tracking and abuse prevention.\",\n  \"properties\": {\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"An external identifier for the user making the request. Should be a UUID, hash, or other opaque identifier.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-metadata-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: Metadata
---
