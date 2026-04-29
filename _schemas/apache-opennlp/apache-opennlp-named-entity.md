---
description: NamedEntity schema from Apache OpenNLP
layout: schema
name: NamedEntity
properties_list:
- description: Entity text
  name: text
  type: string
- description: Entity type
  name: type
  type: string
- description: Start token index
  name: start
  type: integer
- description: End token index (exclusive)
  name: end
  type: integer
- description: Confidence score
  name: probability
  type: number
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-named-entity-schema.json
slug: apache-opennlp-named-entity
source_filename: apache-opennlp-named-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-named-entity-schema.json\",\n  \"title\": \"NamedEntity\",\n  \"description\": \"NamedEntity schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Entity text\",\n      \"example\": \"Pierre Vinken\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Entity type\",\n      \"example\": \"person\",\n      \"enum\": [\n        \"person\",\n        \"location\",\n        \"organization\",\n        \"date\",\n        \"time\",\n        \"money\",\n        \"percent\",\n        \"misc\"\n      ]\n    },\n    \"start\": {\n      \"type\": \"integer\",\n      \"description\": \"Start token index\",\n      \"example\": 0\n    },\n    \"end\": {\n      \"type\": \"integer\",\n\
  \      \"description\": \"End token index (exclusive)\",\n      \"example\": 2\n    },\n    \"probability\": {\n      \"type\": \"number\",\n      \"description\": \"Confidence score\",\n      \"example\": 0.95\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-named-entity-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: NamedEntity
---
