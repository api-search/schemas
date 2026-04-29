---
description: POSTaggingResult schema from Apache OpenNLP
layout: schema
name: POSTaggingResult
properties_list:
- description: ''
  name: tokens
  type: array
- description: POS tags (Penn Treebank tagset)
  name: tags
  type: array
- description: ''
  name: probabilities
  type: array
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-pos-tagging-result-schema.json
slug: apache-opennlp-pos-tagging-result
source_filename: apache-opennlp-pos-tagging-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-pos-tagging-result-schema.json\",\n  \"title\": \"POSTaggingResult\",\n  \"description\": \"POSTaggingResult schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tokens\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"Pierre\",\n        \"Vinken\",\n        \"will\",\n        \"join\"\n      ]\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"POS tags (Penn Treebank tagset)\",\n      \"example\": [\n        \"NNP\",\n        \"NNP\",\n        \"MD\",\n        \"VB\"\n      ]\n    },\n    \"probabilities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"number\"\n      }\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-pos-tagging-result-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: POSTaggingResult
---
