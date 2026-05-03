---
description: Represents a content moderation result classifying text against categories such as hate, harassment, self-harm, sexual content, and violence.
layout: schema
name: OpenAI Moderation Result
properties_list:
- description: Whether the content was flagged as potentially harmful
  name: flagged
  type: boolean
- description: Boolean flags for each moderation category
  name: categories
  type: object
- description: Confidence scores for each moderation category (0-1)
  name: category_scores
  type: object
provider_name: OpenAI APIs
provider_slug: openai-apis
schema_file: json-schema/openai-moderation-schema.json
slug: openai-moderation
source_filename: openai-moderation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.openai.com/schemas/openai/moderation.json\",\n  \"title\": \"OpenAI Moderation Result\",\n  \"description\": \"Represents a content moderation result classifying text against categories such as hate, harassment, self-harm, sexual content, and violence.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flagged\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the content was flagged as potentially harmful\"\n    },\n    \"categories\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"hate\": {\n          \"type\": \"boolean\",\n          \"description\": \"Content expressing hate toward a group\"\n        },\n        \"hate/threatening\": {\n          \"type\": \"boolean\",\n          \"description\": \"Hateful content including violence or threats\"\n        },\n        \"harassment\": {\n          \"type\": \"boolean\",\n          \"description\"\
  : \"Content that harasses a target\"\n        },\n        \"harassment/threatening\": {\n          \"type\": \"boolean\",\n          \"description\": \"Harassment including violence or threats\"\n        },\n        \"self-harm\": {\n          \"type\": \"boolean\",\n          \"description\": \"Content promoting or depicting self-harm\"\n        },\n        \"self-harm/intent\": {\n          \"type\": \"boolean\",\n          \"description\": \"Content expressing intent to self-harm\"\n        },\n        \"self-harm/instructions\": {\n          \"type\": \"boolean\",\n          \"description\": \"Content providing self-harm instructions\"\n        },\n        \"sexual\": {\n          \"type\": \"boolean\",\n          \"description\": \"Sexual content\"\n        },\n        \"sexual/minors\": {\n          \"type\": \"boolean\",\n          \"description\": \"Sexual content involving minors\"\n        },\n        \"violence\": {\n          \"type\": \"boolean\",\n          \"description\"\
  : \"Content depicting violence\"\n        },\n        \"violence/graphic\": {\n          \"type\": \"boolean\",\n          \"description\": \"Graphic violence content\"\n        }\n      },\n      \"description\": \"Boolean flags for each moderation category\"\n    },\n    \"category_scores\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"hate\": { \"type\": \"number\" },\n        \"hate/threatening\": { \"type\": \"number\" },\n        \"harassment\": { \"type\": \"number\" },\n        \"harassment/threatening\": { \"type\": \"number\" },\n        \"self-harm\": { \"type\": \"number\" },\n        \"self-harm/intent\": { \"type\": \"number\" },\n        \"self-harm/instructions\": { \"type\": \"number\" },\n        \"sexual\": { \"type\": \"number\" },\n        \"sexual/minors\": { \"type\": \"number\" },\n        \"violence\": { \"type\": \"number\" },\n        \"violence/graphic\": { \"type\": \"number\" }\n      },\n      \"description\": \"Confidence scores for\
  \ each moderation category (0-1)\"\n    }\n  },\n  \"required\": [\"flagged\", \"categories\", \"category_scores\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/json-schema/openai-moderation-schema.json
tags:
- Artificial Intelligence
- Embeddings
- Image Generation
- Language Models
- Speech
title: OpenAI Moderation Result
---
