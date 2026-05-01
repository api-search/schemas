---
description: Provides information about a PII entity.
layout: schema
name: PiiEntity
properties_list:
- description: ''
  name: Score
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: BeginOffset
  type: object
- description: ''
  name: EndOffset
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-pii-entity-schema.json
slug: openapi.yml-pii-entity
source_filename: openapi.yml-pii-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-pii-entity-schema.json\",\n  \"title\": \"PiiEntity\",\n  \"description\": \"Provides information about a PII entity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Score\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The level of confidence that Amazon Comprehend has in the accuracy of the detection.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PiiEntityType\"\n        },\n        {\n          \"description\": \"The entity's type.\"\n        }\n      ]\n    },\n    \"BeginOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\"\
  : \"The zero-based offset from the beginning of the source text to the first character in the entity.\"\n        }\n      ]\n    },\n    \"EndOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The zero-based offset from the beginning of the source text to the last character in the entity.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-pii-entity-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: PiiEntity
---
