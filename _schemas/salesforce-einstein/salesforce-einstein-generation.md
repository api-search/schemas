---
description: Represents a generative AI content generation result from Einstein GPT, including the generated text, token usage, and content quality assessment.
layout: schema
name: Einstein Generation
properties_list:
- description: Unique generation identifier.
  name: id
  type: string
- description: ID used for submitting feedback on this generation.
  name: generationId
  type: string
- description: The resolved prompt that was sent to the model.
  name: prompt
  type: string
- description: The AI-generated content.
  name: generatedText
  type: string
- description: ID of the model used for generation.
  name: modelId
  type: string
- description: ID of the prompt template used, if any.
  name: promptTemplateId
  type: string
- description: Content quality and safety assessment.
  name: contentQuality
  type: object
- description: Token usage statistics for the generation.
  name: tokenUsage
  type: object
- description: Reason the generation stopped.
  name: finishReason
  type: string
- description: Timestamp when the generation was created.
  name: createdDate
  type: string
provider_name: Salesforce Einstein
provider_slug: salesforce-einstein
schema_file: json-schema/salesforce-einstein-generation-schema.json
slug: salesforce-einstein-generation
source_filename: salesforce-einstein-generation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/salesforce-einstein/json-schema/salesforce-einstein-generation-schema.json\",\n  \"title\": \"Einstein Generation\",\n  \"description\": \"Represents a generative AI content generation result from Einstein GPT, including the generated text, token usage, and content quality assessment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique generation identifier.\"\n    },\n    \"generationId\": {\n      \"type\": \"string\",\n      \"description\": \"ID used for submitting feedback on this generation.\"\n    },\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"The resolved prompt that was sent to the model.\"\n    },\n    \"generatedText\": {\n      \"type\": \"string\",\n      \"description\": \"The AI-generated content.\"\n    },\n    \"modelId\": {\n      \"type\": \"\
  string\",\n      \"description\": \"ID of the model used for generation.\"\n    },\n    \"promptTemplateId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the prompt template used, if any.\"\n    },\n    \"contentQuality\": {\n      \"type\": \"object\",\n      \"description\": \"Content quality and safety assessment.\",\n      \"properties\": {\n        \"scanToxicity\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"isDetected\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether toxic content was detected.\"\n            },\n            \"categories\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"categoryName\": {\n                    \"type\": \"string\",\n                    \"description\": \"Name of the toxicity category.\"\n                  },\n                  \"score\": {\n      \
  \              \"type\": \"number\",\n                    \"description\": \"Toxicity score for this category.\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"tokenUsage\": {\n      \"type\": \"object\",\n      \"description\": \"Token usage statistics for the generation.\",\n      \"properties\": {\n        \"promptTokens\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of tokens in the prompt.\"\n        },\n        \"completionTokens\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of tokens in the generated response.\"\n        },\n        \"totalTokens\": {\n          \"type\": \"integer\",\n          \"description\": \"Total tokens used.\"\n        }\n      }\n    },\n    \"finishReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason the generation stopped.\",\n      \"enum\": [\"stop\", \"length\", \"content_filter\"]\n    },\n    \"\
  createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the generation was created.\"\n    }\n  },\n  \"required\": [\"generationId\", \"generatedText\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/json-schema/salesforce-einstein-generation-schema.json
tags:
- Artificial Intelligence
- Computer Vision
- CRM
- Machine Learning
- Natural Language Processing
- Predictive Analytics
- Salesforce
title: Einstein Generation
---
