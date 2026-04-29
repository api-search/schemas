---
description: LemmatizationResult schema from Apache OpenNLP
layout: schema
name: LemmatizationResult
properties_list:
- description: ''
  name: tokens
  type: array
- description: ''
  name: lemmas
  type: array
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-lemmatization-result-schema.json
slug: apache-opennlp-lemmatization-result
source_filename: apache-opennlp-lemmatization-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-lemmatization-result-schema.json\",\n  \"title\": \"LemmatizationResult\",\n  \"description\": \"LemmatizationResult schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tokens\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"running\",\n        \"faster\"\n      ]\n    },\n    \"lemmas\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"run\",\n        \"fast\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-lemmatization-result-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: LemmatizationResult
---
