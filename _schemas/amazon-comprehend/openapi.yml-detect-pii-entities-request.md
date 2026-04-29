---
description: DetectPiiEntitiesRequest schema
layout: schema
name: DetectPiiEntitiesRequest
properties_list:
- description: ''
  name: Text
  type: object
- description: ''
  name: LanguageCode
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-detect-pii-entities-request-schema.json
slug: openapi.yml-detect-pii-entities-request
source_filename: openapi.yml-detect-pii-entities-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-pii-entities-request-schema.json\",\n  \"title\": \"DetectPiiEntitiesRequest\",\n  \"description\": \"DetectPiiEntitiesRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Text\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A UTF-8 text string. The maximum string size is 100 KB.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"description\": \"The language of the input documents. Currently, English is the only valid language.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Text\",\n    \"LanguageCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-pii-entities-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DetectPiiEntitiesRequest
---
