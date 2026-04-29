---
description: Describes the level of confidence that Amazon Comprehend has in the accuracy of its detection of sentiments.
layout: schema
name: SentimentScore
properties_list:
- description: ''
  name: Positive
  type: object
- description: ''
  name: Negative
  type: object
- description: ''
  name: Neutral
  type: object
- description: ''
  name: Mixed
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-sentiment-score-schema.json
slug: openapi.yml-sentiment-score
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-sentiment-score-schema.json\",\n  \"title\": \"SentimentScore\",\n  \"description\": \"Describes the level of confidence that Amazon Comprehend has in the accuracy of its detection of sentiments.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Positive\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The level of confidence that Amazon Comprehend has in the accuracy of its detection of the <code>POSITIVE</code> sentiment.\"\n        }\n      ]\n    },\n    \"Negative\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The level of confidence that Amazon Comprehend has in the accuracy of its detection of\
  \ the <code>NEGATIVE</code> sentiment.\"\n        }\n      ]\n    },\n    \"Neutral\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The level of confidence that Amazon Comprehend has in the accuracy of its detection of the <code>NEUTRAL</code> sentiment.\"\n        }\n      ]\n    },\n    \"Mixed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The level of confidence that Amazon Comprehend has in the accuracy of its detection of the <code>MIXED</code> sentiment.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-sentiment-score-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: SentimentScore
---
