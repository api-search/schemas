---
description: BatchDetectSyntaxRequest schema
layout: schema
name: BatchDetectSyntaxRequest
properties_list:
- description: ''
  name: TextList
  type: object
- description: ''
  name: LanguageCode
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-batch-detect-syntax-request-schema.json
slug: openapi.yml-batch-detect-syntax-request
source_filename: openapi.yml-batch-detect-syntax-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-batch-detect-syntax-request-schema.json\",\n  \"title\": \"BatchDetectSyntaxRequest\",\n  \"description\": \"BatchDetectSyntaxRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TextList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerInputStringList\"\n        },\n        {\n          \"description\": \"A list containing the UTF-8 encoded text of the input documents. The list can contain a maximum of 25 documents. The maximum size for each document is 5 KB.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntaxLanguageCode\"\n        },\n        {\n          \"description\": \"The language of the input documents. You can specify any of the following\
  \ languages supported by Amazon Comprehend: German (\\\"de\\\"), English (\\\"en\\\"), Spanish (\\\"es\\\"), French (\\\"fr\\\"), Italian (\\\"it\\\"), or Portuguese (\\\"pt\\\"). All documents must be in the same language.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TextList\",\n    \"LanguageCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-batch-detect-syntax-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: BatchDetectSyntaxRequest
---
