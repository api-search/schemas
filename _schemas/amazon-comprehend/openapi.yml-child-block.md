---
description: Nested block contained within a block.
layout: schema
name: ChildBlock
properties_list:
- description: ''
  name: ChildBlockId
  type: object
- description: ''
  name: BeginOffset
  type: object
- description: ''
  name: EndOffset
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-child-block-schema.json
slug: openapi.yml-child-block
source_filename: openapi.yml-child-block-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-child-block-schema.json\",\n  \"title\": \"ChildBlock\",\n  \"description\": \"Nested block contained within a block.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChildBlockId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Unique identifier for the child block.\"\n        }\n      ]\n    },\n    \"BeginOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Offset of the start of the child block within its parent block.\"\n        }\n      ]\n    },\n    \"EndOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\"\
  : \"Offset of the end of the child block within its parent block.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-child-block-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ChildBlock
---
