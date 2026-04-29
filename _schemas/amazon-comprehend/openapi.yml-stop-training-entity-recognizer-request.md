---
description: StopTrainingEntityRecognizerRequest schema
layout: schema
name: StopTrainingEntityRecognizerRequest
properties_list:
- description: ''
  name: EntityRecognizerArn
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-stop-training-entity-recognizer-request-schema.json
slug: openapi.yml-stop-training-entity-recognizer-request
source_filename: openapi.yml-stop-training-entity-recognizer-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-stop-training-entity-recognizer-request-schema.json\",\n  \"title\": \"StopTrainingEntityRecognizerRequest\",\n  \"description\": \"StopTrainingEntityRecognizerRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EntityRecognizerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityRecognizerArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the entity recognizer currently being trained.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EntityRecognizerArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-stop-training-entity-recognizer-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: StopTrainingEntityRecognizerRequest
---
