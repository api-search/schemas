---
description: A reference to a block.
layout: schema
name: BlockReference
properties_list:
- description: ''
  name: BlockId
  type: object
- description: ''
  name: BeginOffset
  type: object
- description: ''
  name: EndOffset
  type: object
- description: ''
  name: ChildBlocks
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-block-reference-schema.json
slug: openapi.yml-block-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-block-reference-schema.json\",\n  \"title\": \"BlockReference\",\n  \"description\": \"A reference to a block. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BlockId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Unique identifier for the block.\"\n        }\n      ]\n    },\n    \"BeginOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Offset of the start of the block within its parent block.\"\n        }\n      ]\n    },\n    \"EndOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Offset of\
  \ the end of the block within its parent block.\"\n        }\n      ]\n    },\n    \"ChildBlocks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfChildBlocks\"\n        },\n        {\n          \"description\": \"List of child blocks within this block.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-block-reference-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: BlockReference
---
