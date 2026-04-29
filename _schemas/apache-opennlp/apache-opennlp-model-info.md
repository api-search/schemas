---
description: ModelInfo schema from Apache OpenNLP
layout: schema
name: ModelInfo
properties_list:
- description: Unique model identifier
  name: modelId
  type: string
- description: Model language
  name: language
  type: string
- description: Model type
  name: type
  type: string
- description: Model version
  name: version
  type: string
- description: Whether model is currently loaded
  name: loaded
  type: boolean
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-model-info-schema.json
slug: apache-opennlp-model-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-model-info-schema.json\",\n  \"title\": \"ModelInfo\",\n  \"description\": \"ModelInfo schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"modelId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique model identifier\",\n      \"example\": \"en-ner-person.bin\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Model language\",\n      \"example\": \"eng\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Model type\",\n      \"example\": \"TokenNameFinder\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Model version\",\n      \"example\": 1.5\n    },\n    \"loaded\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether model is currently\
  \ loaded\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-model-info-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: ModelInfo
---
