---
description: <p>Provides information about an entity. </p> <p> </p>
layout: schema
name: Entity
properties_list:
- description: ''
  name: Score
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Text
  type: object
- description: ''
  name: BeginOffset
  type: object
- description: ''
  name: EndOffset
  type: object
- description: ''
  name: BlockReferences
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-entity-schema.json
slug: openapi.yml-entity
source_filename: openapi.yml-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-schema.json\",\n  \"title\": \"Entity\",\n  \"description\": \"<p>Provides information about an entity. </p> <p> </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Score\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The level of confidence that Amazon Comprehend has in the accuracy of the detection.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityType\"\n        },\n        {\n          \"description\": \"<p>The entity type. For entity detection using the built-in model, this field contains one of the standard entity types listed below.</p> <p>For custom entity detection, this field contains one of the\
  \ entity types that you specified when you trained your custom model.</p>\"\n        }\n      ]\n    },\n    \"Text\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The text of the entity.\"\n        }\n      ]\n    },\n    \"BeginOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"<p>The zero-based offset from the beginning of the source text to the first character in the entity.</p> <p>This field is empty for non-text input.</p>\"\n        }\n      ]\n    },\n    \"EndOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"<p>The zero-based offset from the beginning of the source text to the last character in the entity.</p> <p>This field is empty for non-text input.</p>\"\n        }\n      ]\n    },\n \
  \   \"BlockReferences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfBlockReferences\"\n        },\n        {\n          \"description\": \"A reference to each block for this entity. This field is empty for plain-text input.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: Entity
---
