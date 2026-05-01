---
description: DetectDominantLanguageRequest schema
layout: schema
name: DetectDominantLanguageRequest
properties_list:
- description: ''
  name: Text
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-detect-dominant-language-request-schema.json
slug: openapi.yml-detect-dominant-language-request
source_filename: openapi.yml-detect-dominant-language-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-dominant-language-request-schema.json\",\n  \"title\": \"DetectDominantLanguageRequest\",\n  \"description\": \"DetectDominantLanguageRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Text\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerInputString\"\n        },\n        {\n          \"description\": \"A UTF-8 text string. The string must contain at least 20 characters. The maximum string size is 100 KB.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Text\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-dominant-language-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DetectDominantLanguageRequest
---
