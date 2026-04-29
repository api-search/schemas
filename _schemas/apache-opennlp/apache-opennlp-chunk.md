---
description: Chunk schema from Apache OpenNLP
layout: schema
name: Chunk
properties_list:
- description: Chunk text
  name: text
  type: string
- description: Chunk type
  name: type
  type: string
- description: ''
  name: start
  type: integer
- description: ''
  name: end
  type: integer
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-chunk-schema.json
slug: apache-opennlp-chunk
source_filename: apache-opennlp-chunk-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-chunk-schema.json\",\n  \"title\": \"Chunk\",\n  \"description\": \"Chunk schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Chunk text\",\n      \"example\": \"Pierre Vinken\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Chunk type\",\n      \"example\": \"NP\",\n      \"enum\": [\n        \"NP\",\n        \"VP\",\n        \"PP\",\n        \"ADJP\",\n        \"ADVP\",\n        \"SBAR\",\n        \"PRT\",\n        \"CONJP\",\n        \"INTJ\",\n        \"LST\",\n        \"UCP\"\n      ]\n    },\n    \"start\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    },\n    \"end\": {\n      \"type\": \"integer\",\n      \"example\": 2\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-chunk-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: Chunk
---
