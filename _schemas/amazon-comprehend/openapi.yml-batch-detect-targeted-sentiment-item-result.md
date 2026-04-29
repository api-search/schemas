---
description: Analysis results for one of the documents in the batch.
layout: schema
name: BatchDetectTargetedSentimentItemResult
properties_list:
- description: ''
  name: Index
  type: object
- description: ''
  name: Entities
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-batch-detect-targeted-sentiment-item-result-schema.json
slug: openapi.yml-batch-detect-targeted-sentiment-item-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-batch-detect-targeted-sentiment-item-result-schema.json\",\n  \"title\": \"BatchDetectTargetedSentimentItemResult\",\n  \"description\": \"Analysis results for one of the documents in the batch.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Index\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The zero-based index of this result in the input list.\"\n        }\n      ]\n    },\n    \"Entities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfTargetedSentimentEntities\"\n        },\n        {\n          \"description\": \"An array of targeted sentiment entities.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-batch-detect-targeted-sentiment-item-result-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: BatchDetectTargetedSentimentItemResult
---
