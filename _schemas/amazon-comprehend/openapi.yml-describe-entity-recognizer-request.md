---
description: DescribeEntityRecognizerRequest schema
layout: schema
name: DescribeEntityRecognizerRequest
properties_list:
- description: ''
  name: EntityRecognizerArn
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-describe-entity-recognizer-request-schema.json
slug: openapi.yml-describe-entity-recognizer-request
source_filename: openapi.yml-describe-entity-recognizer-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-entity-recognizer-request-schema.json\",\n  \"title\": \"DescribeEntityRecognizerRequest\",\n  \"description\": \"DescribeEntityRecognizerRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EntityRecognizerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityRecognizerArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the entity recognizer.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EntityRecognizerArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-entity-recognizer-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DescribeEntityRecognizerRequest
---
