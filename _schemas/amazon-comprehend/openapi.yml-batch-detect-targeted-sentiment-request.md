---
description: BatchDetectTargetedSentimentRequest schema
layout: schema
name: BatchDetectTargetedSentimentRequest
properties_list:
- description: ''
  name: TextList
  type: object
- description: ''
  name: LanguageCode
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-batch-detect-targeted-sentiment-request-schema.json
slug: openapi.yml-batch-detect-targeted-sentiment-request
source_filename: openapi.yml-batch-detect-targeted-sentiment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-batch-detect-targeted-sentiment-request-schema.json\",\n  \"title\": \"BatchDetectTargetedSentimentRequest\",\n  \"description\": \"BatchDetectTargetedSentimentRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TextList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerInputStringList\"\n        },\n        {\n          \"description\": \"A list containing the UTF-8 encoded text of the input documents. The list can contain a maximum of 25 documents. The maximum size of each document is 5 KB.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"description\": \"The language of the input documents. Currently,\
  \ English is the only supported language.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TextList\",\n    \"LanguageCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-batch-detect-targeted-sentiment-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: BatchDetectTargetedSentimentRequest
---
