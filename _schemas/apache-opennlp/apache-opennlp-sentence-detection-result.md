---
description: SentenceDetectionResult schema from Apache OpenNLP
layout: schema
name: SentenceDetectionResult
properties_list:
- description: Detected sentences
  name: sentences
  type: array
- description: ''
  name: spans
  type: array
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-sentence-detection-result-schema.json
slug: apache-opennlp-sentence-detection-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-sentence-detection-result-schema.json\",\n  \"title\": \"SentenceDetectionResult\",\n  \"description\": \"SentenceDetectionResult schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sentences\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Detected sentences\",\n      \"example\": [\n        \"Pierre Vinken will join the board.\",\n        \"He is 61 years old.\"\n      ]\n    },\n    \"spans\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Span\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-sentence-detection-result-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: SentenceDetectionResult
---
