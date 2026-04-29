---
description: Represents a work in the input text that was recognized and assigned a part of speech. There is one syntax token record for each word in the source text.
layout: schema
name: SyntaxToken
properties_list:
- description: ''
  name: TokenId
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
  name: PartOfSpeech
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-syntax-token-schema.json
slug: openapi.yml-syntax-token
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-syntax-token-schema.json\",\n  \"title\": \"SyntaxToken\",\n  \"description\": \"Represents a work in the input text that was recognized and assigned a part of speech. There is one syntax token record for each word in the source text.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TokenId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"A unique identifier for a token.\"\n        }\n      ]\n    },\n    \"Text\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The word that was recognized in the source text.\"\n        }\n      ]\n    },\n    \"BeginOffset\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The zero-based offset from the beginning of the source text to the first character in the word.\"\n        }\n      ]\n    },\n    \"EndOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The zero-based offset from the beginning of the source text to the last character in the word.\"\n        }\n      ]\n    },\n    \"PartOfSpeech\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PartOfSpeechTag\"\n        },\n        {\n          \"description\": \"Provides the part of speech label and the confidence level that Amazon Comprehend has that the part of speech was correctly identified. For more information, see <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/how-syntax.html\\\">Syntax</a> in the Comprehend Developer Guide. \"\n        }\n      ]\n \
  \   }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-syntax-token-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: SyntaxToken
---
