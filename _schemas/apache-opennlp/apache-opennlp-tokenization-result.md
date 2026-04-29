---
description: TokenizationResult schema from Apache OpenNLP
layout: schema
name: TokenizationResult
properties_list:
- description: Extracted tokens
  name: tokens
  type: array
- description: ''
  name: spans
  type: array
- description: Confidence for each token boundary
  name: probabilities
  type: array
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-tokenization-result-schema.json
slug: apache-opennlp-tokenization-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-tokenization-result-schema.json\",\n  \"title\": \"TokenizationResult\",\n  \"description\": \"TokenizationResult schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tokens\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Extracted tokens\",\n      \"example\": [\n        \"Pierre\",\n        \"Vinken\",\n        \",\",\n        \"61\",\n        \"years\",\n        \"old\"\n      ]\n    },\n    \"spans\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Span\"\n      }\n    },\n    \"probabilities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"number\"\n      },\n      \"description\": \"Confidence for each token boundary\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-tokenization-result-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: TokenizationResult
---
