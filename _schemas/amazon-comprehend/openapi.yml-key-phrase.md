---
description: Describes a key noun phrase.
layout: schema
name: KeyPhrase
properties_list:
- description: ''
  name: Score
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
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-key-phrase-schema.json
slug: openapi.yml-key-phrase
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-key-phrase-schema.json\",\n  \"title\": \"KeyPhrase\",\n  \"description\": \"Describes a key noun phrase.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Score\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The level of confidence that Amazon Comprehend has in the accuracy of the detection.\"\n        }\n      ]\n    },\n    \"Text\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The text of a key noun phrase.\"\n        }\n      ]\n    },\n    \"BeginOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\":\
  \ \"The zero-based offset from the beginning of the source text to the first character in the key phrase.\"\n        }\n      ]\n    },\n    \"EndOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The zero-based offset from the beginning of the source text to the last character in the key phrase.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-key-phrase-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: KeyPhrase
---
