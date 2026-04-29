---
description: Span schema from Apache OpenNLP
layout: schema
name: Span
properties_list:
- description: Start character offset
  name: start
  type: integer
- description: End character offset (exclusive)
  name: end
  type: integer
- description: Span type if applicable
  name: type
  type: string
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-span-schema.json
slug: apache-opennlp-span
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-span-schema.json\",\n  \"title\": \"Span\",\n  \"description\": \"Span schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"start\": {\n      \"type\": \"integer\",\n      \"description\": \"Start character offset\",\n      \"example\": 0\n    },\n    \"end\": {\n      \"type\": \"integer\",\n      \"description\": \"End character offset (exclusive)\",\n      \"example\": 13\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Span type if applicable\",\n      \"example\": \"person\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-span-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: Span
---
