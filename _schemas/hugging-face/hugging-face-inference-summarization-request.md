---
description: ''
layout: schema
name: SummarizationRequest
properties_list:
- description: The text to summarize
  name: inputs
  type: string
- description: ''
  name: parameters
  type: object
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-summarization-request-schema.json
slug: hugging-face-inference-summarization-request
source_filename: hugging-face-inference-summarization-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SummarizationRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"string\",\n      \"description\": \"The text to summarize\"\n    },\n    \"parameters\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-summarization-request-schema.json
tags: []
title: SummarizationRequest
---
