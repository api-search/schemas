---
description: ImportModelResponse schema
layout: schema
name: ImportModelResponse
properties_list:
- description: ''
  name: ModelArn
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-import-model-response-schema.json
slug: openapi.yml-import-model-response
source_filename: openapi.yml-import-model-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-import-model-response-schema.json\",\n  \"title\": \"ImportModelResponse\",\n  \"description\": \"ImportModelResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendModelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the custom model being imported.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-import-model-response-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ImportModelResponse
---
