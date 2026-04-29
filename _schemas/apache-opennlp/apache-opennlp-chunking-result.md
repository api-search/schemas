---
description: ChunkingResult schema from Apache OpenNLP
layout: schema
name: ChunkingResult
properties_list:
- description: ''
  name: chunks
  type: array
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-chunking-result-schema.json
slug: apache-opennlp-chunking-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-chunking-result-schema.json\",\n  \"title\": \"ChunkingResult\",\n  \"description\": \"ChunkingResult schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"chunks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Chunk\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-chunking-result-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: ChunkingResult
---
