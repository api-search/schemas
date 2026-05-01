---
description: DescribeEntityRecognizerResponse schema
layout: schema
name: DescribeEntityRecognizerResponse
properties_list:
- description: ''
  name: EntityRecognizerProperties
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-describe-entity-recognizer-response-schema.json
slug: openapi.yml-describe-entity-recognizer-response
source_filename: openapi.yml-describe-entity-recognizer-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-entity-recognizer-response-schema.json\",\n  \"title\": \"DescribeEntityRecognizerResponse\",\n  \"description\": \"DescribeEntityRecognizerResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EntityRecognizerProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityRecognizerProperties\"\n        },\n        {\n          \"description\": \"Describes information associated with an entity recognizer.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-entity-recognizer-response-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DescribeEntityRecognizerResponse
---
