---
description: DetectSyntaxRequest schema
layout: schema
name: DetectSyntaxRequest
properties_list:
- description: ''
  name: Text
  type: object
- description: ''
  name: LanguageCode
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-detect-syntax-request-schema.json
slug: openapi.yml-detect-syntax-request
source_filename: openapi.yml-detect-syntax-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-syntax-request-schema.json\",\n  \"title\": \"DetectSyntaxRequest\",\n  \"description\": \"DetectSyntaxRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Text\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerInputString\"\n        },\n        {\n          \"description\": \"A UTF-8 string. The maximum string size is 5 KB.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntaxLanguageCode\"\n        },\n        {\n          \"description\": \"The language code of the input documents. You can specify any of the following languages supported by Amazon Comprehend: German (\\\"de\\\"), English (\\\"en\\\"), Spanish (\\\"es\\\"), French (\\\"fr\\\"\
  ), Italian (\\\"it\\\"), or Portuguese (\\\"pt\\\").\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Text\",\n    \"LanguageCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-syntax-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DetectSyntaxRequest
---
