---
description: The result of calling the operation. The operation returns one object that is successfully processed by the operation.
layout: schema
name: BatchDetectSyntaxItemResult
properties_list:
- description: ''
  name: Index
  type: object
- description: ''
  name: SyntaxTokens
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-batch-detect-syntax-item-result-schema.json
slug: openapi.yml-batch-detect-syntax-item-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-batch-detect-syntax-item-result-schema.json\",\n  \"title\": \"BatchDetectSyntaxItemResult\",\n  \"description\": \"The result of calling the operation. The operation returns one object that is successfully processed by the operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Index\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The zero-based index of the document in the input list.\"\n        }\n      ]\n    },\n    \"SyntaxTokens\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfSyntaxTokens\"\n        },\n        {\n          \"description\": \"The syntax tokens for the words in the document, one token for each word.\"\n        }\n      ]\n \
  \   }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-batch-detect-syntax-item-result-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: BatchDetectSyntaxItemResult
---
