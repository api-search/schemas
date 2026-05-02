---
description: Results from an IBM Natural Language Understanding analysis.
layout: schema
name: NLU Analysis
properties_list:
- description: The detected language of the analyzed text.
  name: language
  type: string
- description: The text that was analyzed.
  name: analyzed_text
  type: string
- description: Document-level sentiment analysis.
  name: sentiment
  type: object
- description: Document-level emotion analysis.
  name: emotion
  type: object
- description: Detected entities.
  name: entities
  type: array
- description: Extracted keywords.
  name: keywords
  type: array
- description: Content categories.
  name: categories
  type: array
- description: High-level concepts.
  name: concepts
  type: array
provider_name: International Business Machines
provider_slug: international-business-machines
schema_file: json-schema/nlu-analysis.json
slug: nlu-analysis
source_filename: nlu-analysis.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"nlu-analysis.json\",\n  \"title\": \"NLU Analysis\",\n  \"description\": \"Results from an IBM Natural Language Understanding analysis.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"The detected language of the analyzed text.\"\n    },\n    \"analyzed_text\": {\n      \"type\": \"string\",\n      \"description\": \"The text that was analyzed.\"\n    },\n    \"sentiment\": {\n      \"type\": \"object\",\n      \"description\": \"Document-level sentiment analysis.\",\n      \"properties\": {\n        \"document\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"score\": {\n              \"type\": \"number\",\n              \"minimum\": -1,\n              \"maximum\": 1\n            },\n            \"label\": {\n              \"type\": \"string\",\n              \"enum\": [\"positive\", \"\
  negative\", \"neutral\"]\n            }\n          }\n        }\n      }\n    },\n    \"emotion\": {\n      \"type\": \"object\",\n      \"description\": \"Document-level emotion analysis.\",\n      \"properties\": {\n        \"document\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"emotion\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"sadness\": { \"type\": \"number\" },\n                \"joy\": { \"type\": \"number\" },\n                \"fear\": { \"type\": \"number\" },\n                \"disgust\": { \"type\": \"number\" },\n                \"anger\": { \"type\": \"number\" }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"entities\": {\n      \"type\": \"array\",\n      \"description\": \"Detected entities.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": { \"type\": \"string\" },\n          \"text\": { \"type\":\
  \ \"string\" },\n          \"relevance\": { \"type\": \"number\" },\n          \"count\": { \"type\": \"integer\" },\n          \"confidence\": { \"type\": \"number\" }\n        }\n      }\n    },\n    \"keywords\": {\n      \"type\": \"array\",\n      \"description\": \"Extracted keywords.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"text\": { \"type\": \"string\" },\n          \"relevance\": { \"type\": \"number\" },\n          \"count\": { \"type\": \"integer\" }\n        }\n      }\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"description\": \"Content categories.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"label\": { \"type\": \"string\" },\n          \"score\": { \"type\": \"number\" }\n        }\n      }\n    },\n    \"concepts\": {\n      \"type\": \"array\",\n      \"description\": \"High-level concepts.\",\n      \"items\": {\n        \"type\": \"object\",\n\
  \        \"properties\": {\n          \"text\": { \"type\": \"string\" },\n          \"relevance\": { \"type\": \"number\" },\n          \"dbpedia_resource\": { \"type\": \"string\" }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/json-schema/nlu-analysis.json
tags:
- Artificial Intelligence
- Cloud
- Enterprise
- IBM
title: NLU Analysis
---
