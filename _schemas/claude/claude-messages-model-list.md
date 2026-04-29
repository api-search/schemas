---
description: Paginated list of available models.
layout: schema
name: ModelList
properties_list:
- description: ''
  name: data
  type: array
- description: Whether there are more results available.
  name: has_more
  type: boolean
- description: ID of the first item. Use as before_id for the previous page.
  name: first_id
  type: string
- description: ID of the last item. Use as after_id for the next page.
  name: last_id
  type: string
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-model-list-schema.json
slug: claude-messages-model-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ModelList\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of available models.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\"\n    },\n    \"has_more\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether there are more results available.\"\n    },\n    \"first_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the first item. Use as before_id for the previous page.\"\n    },\n    \"last_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the last item. Use as after_id for the next page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-model-list-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: ModelList
---
