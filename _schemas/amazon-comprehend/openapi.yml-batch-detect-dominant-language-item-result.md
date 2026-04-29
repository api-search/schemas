---
description: The result of calling the operation. The operation returns one object for each document that is successfully processed by the operation.
layout: schema
name: BatchDetectDominantLanguageItemResult
properties_list:
- description: ''
  name: Index
  type: object
- description: ''
  name: Languages
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-batch-detect-dominant-language-item-result-schema.json
slug: openapi.yml-batch-detect-dominant-language-item-result
source_filename: openapi.yml-batch-detect-dominant-language-item-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-batch-detect-dominant-language-item-result-schema.json\",\n  \"title\": \"BatchDetectDominantLanguageItemResult\",\n  \"description\": \"The result of calling the operation. The operation returns one object for each document that is successfully processed by the operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Index\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The zero-based index of the document in the input list.\"\n        }\n      ]\n    },\n    \"Languages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfDominantLanguages\"\n        },\n        {\n          \"description\": \"One or more <a>DominantLanguage</a> objects describing the\
  \ dominant languages in the document.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-batch-detect-dominant-language-item-result-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: BatchDetectDominantLanguageItemResult
---
