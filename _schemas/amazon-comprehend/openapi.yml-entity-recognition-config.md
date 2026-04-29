---
description: Configuration required for an entity recognition model.
layout: schema
name: EntityRecognitionConfig
properties_list:
- description: ''
  name: EntityTypes
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-entity-recognition-config-schema.json
slug: openapi.yml-entity-recognition-config
source_filename: openapi.yml-entity-recognition-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-recognition-config-schema.json\",\n  \"title\": \"EntityRecognitionConfig\",\n  \"description\": \"Configuration required for an entity recognition model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EntityTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityTypesList\"\n        },\n        {\n          \"description\": \"Up to 25 entity types that the model is trained to recognize.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EntityTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-recognition-config-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: EntityRecognitionConfig
---
