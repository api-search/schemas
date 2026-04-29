---
description: DetectTargetedSentimentRequest schema
layout: schema
name: DetectTargetedSentimentRequest
properties_list:
- description: ''
  name: Text
  type: object
- description: ''
  name: LanguageCode
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-detect-targeted-sentiment-request-schema.json
slug: openapi.yml-detect-targeted-sentiment-request
source_filename: openapi.yml-detect-targeted-sentiment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-targeted-sentiment-request-schema.json\",\n  \"title\": \"DetectTargetedSentimentRequest\",\n  \"description\": \"DetectTargetedSentimentRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Text\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerInputString\"\n        },\n        {\n          \"description\": \"A UTF-8 text string. The maximum string length is 5 KB.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"description\": \"The language of the input documents. Currently, English is the only supported language.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Text\",\n    \"LanguageCode\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-targeted-sentiment-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DetectTargetedSentimentRequest
---
