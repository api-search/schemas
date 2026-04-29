---
description: DetectTargetedSentimentResponse schema
layout: schema
name: DetectTargetedSentimentResponse
properties_list:
- description: ''
  name: Entities
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-detect-targeted-sentiment-response-schema.json
slug: openapi.yml-detect-targeted-sentiment-response
source_filename: openapi.yml-detect-targeted-sentiment-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-targeted-sentiment-response-schema.json\",\n  \"title\": \"DetectTargetedSentimentResponse\",\n  \"description\": \"DetectTargetedSentimentResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Entities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfTargetedSentimentEntities\"\n        },\n        {\n          \"description\": \"Targeted sentiment analysis for each of the entities identified in the input text.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-targeted-sentiment-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DetectTargetedSentimentResponse
---
