---
description: DetectSentimentResponse schema
layout: schema
name: DetectSentimentResponse
properties_list:
- description: ''
  name: Sentiment
  type: object
- description: ''
  name: SentimentScore
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-detect-sentiment-response-schema.json
slug: openapi.yml-detect-sentiment-response
source_filename: openapi.yml-detect-sentiment-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-sentiment-response-schema.json\",\n  \"title\": \"DetectSentimentResponse\",\n  \"description\": \"DetectSentimentResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Sentiment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SentimentType\"\n        },\n        {\n          \"description\": \"The inferred sentiment that Amazon Comprehend has the highest level of confidence in.\"\n        }\n      ]\n    },\n    \"SentimentScore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SentimentScore\"\n        },\n        {\n          \"description\": \"An object that lists the sentiments, and their corresponding confidence levels.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-sentiment-response-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DetectSentimentResponse
---
