---
description: TextRequest schema from Apache OpenNLP
layout: schema
name: TextRequest
properties_list:
- description: Input text to process
  name: text
  type: string
- description: ISO-639-3 language code hint
  name: language
  type: string
- description: Specific model to use (optional)
  name: modelId
  type: string
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-text-request-schema.json
slug: apache-opennlp-text-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-text-request-schema.json\",\n  \"title\": \"TextRequest\",\n  \"description\": \"TextRequest schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Input text to process\",\n      \"example\": \"Pierre Vinken, 61 years old, will join the board as a nonexecutive director Nov. 29.\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"ISO-639-3 language code hint\",\n      \"example\": \"eng\"\n    },\n    \"modelId\": {\n      \"type\": \"string\",\n      \"description\": \"Specific model to use (optional)\",\n      \"example\": \"en-sent.bin\"\n    }\n  },\n  \"required\": [\n    \"text\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-text-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: TextRequest
---
