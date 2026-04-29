---
description: A document content block for PDFs and text documents.
layout: schema
name: DocumentBlockParam
properties_list:
- description: ''
  name: type
  type: string
- description: The source of the document.
  name: source
  type: object
- description: Optional title for the document.
  name: title
  type: string
- description: Optional context about the document.
  name: context
  type: string
- description: Citation configuration for the document.
  name: citations
  type: object
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-document-block-param-schema.json
slug: claude-messages-document-block-param
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DocumentBlockParam\",\n  \"type\": \"object\",\n  \"description\": \"A document content block for PDFs and text documents.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"source\": {\n      \"type\": \"object\",\n      \"description\": \"The source of the document.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Optional title for the document.\"\n    },\n    \"context\": {\n      \"type\": \"string\",\n      \"description\": \"Optional context about the document.\"\n    },\n    \"citations\": {\n      \"type\": \"object\",\n      \"description\": \"Citation configuration for the document.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-document-block-param-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: DocumentBlockParam
---
