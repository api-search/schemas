---
description: ''
layout: schema
name: QuestionAnsweringResponse
properties_list:
- description: The extracted answer
  name: answer
  type: string
- description: Confidence score
  name: score
  type: number
- description: Start character position in context
  name: start
  type: integer
- description: End character position in context
  name: end
  type: integer
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-question-answering-response-schema.json
slug: hugging-face-inference-question-answering-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QuestionAnsweringResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"answer\": {\n      \"type\": \"string\",\n      \"description\": \"The extracted answer\"\n    },\n    \"score\": {\n      \"type\": \"number\",\n      \"description\": \"Confidence score\"\n    },\n    \"start\": {\n      \"type\": \"integer\",\n      \"description\": \"Start character position in context\"\n    },\n    \"end\": {\n      \"type\": \"integer\",\n      \"description\": \"End character position in context\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-question-answering-response-schema.json
tags: []
title: QuestionAnsweringResponse
---
