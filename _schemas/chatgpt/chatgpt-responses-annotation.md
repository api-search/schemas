---
description: ''
layout: schema
name: Annotation
properties_list:
- description: The type of annotation.
  name: type
  type: string
- description: The start index of the annotation in the text.
  name: start_index
  type: integer
- description: The end index of the annotation in the text.
  name: end_index
  type: integer
- description: The URL cited. Present for url_citation type.
  name: url
  type: string
- description: The title of the cited resource.
  name: title
  type: string
- description: The ID of the cited file. Present for file_citation and file_path types.
  name: file_id
  type: string
- description: The relevant quote from the file.
  name: quote
  type: string
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-responses-annotation-schema.json
slug: chatgpt-responses-annotation
source_filename: chatgpt-responses-annotation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Annotation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of annotation.\"\n    },\n    \"start_index\": {\n      \"type\": \"integer\",\n      \"description\": \"The start index of the annotation in the text.\"\n    },\n    \"end_index\": {\n      \"type\": \"integer\",\n      \"description\": \"The end index of the annotation in the text.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL cited. Present for url_citation type.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the cited resource.\"\n    },\n    \"file_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the cited file. Present for file_citation and\\nfile_path types.\\n\"\n    },\n    \"quote\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The relevant quote from the file.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-responses-annotation-schema.json
tags:
- Agents
- AI
- ChatGPT
- Embeddings
- Fine-Tuning
- GPT-4
- GPT-5
- Language Model
- OpenAI
- Realtime
title: Annotation
---
