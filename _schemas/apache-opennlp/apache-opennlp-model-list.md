---
description: ModelList schema from Apache OpenNLP
layout: schema
name: ModelList
properties_list:
- description: ''
  name: models
  type: array
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-model-list-schema.json
slug: apache-opennlp-model-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-model-list-schema.json\",\n  \"title\": \"ModelList\",\n  \"description\": \"ModelList schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"models\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ModelInfo\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-model-list-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: ModelList
---
