---
description: NERResult schema from Apache OpenNLP
layout: schema
name: NERResult
properties_list:
- description: ''
  name: entities
  type: array
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-ner-result-schema.json
slug: apache-opennlp-ner-result
source_filename: apache-opennlp-ner-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-ner-result-schema.json\",\n  \"title\": \"NERResult\",\n  \"description\": \"NERResult schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/NamedEntity\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-ner-result-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: NERResult
---
