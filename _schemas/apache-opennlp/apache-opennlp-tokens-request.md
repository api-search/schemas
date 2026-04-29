---
description: TokensRequest schema from Apache OpenNLP
layout: schema
name: TokensRequest
properties_list:
- description: Pre-tokenized array of text tokens
  name: tokens
  type: array
- description: ISO-639-3 language code
  name: language
  type: string
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-tokens-request-schema.json
slug: apache-opennlp-tokens-request
source_filename: apache-opennlp-tokens-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-tokens-request-schema.json\",\n  \"title\": \"TokensRequest\",\n  \"description\": \"TokensRequest schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tokens\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Pre-tokenized array of text tokens\",\n      \"example\": [\n        \"Pierre\",\n        \"Vinken\",\n        \"will\",\n        \"join\",\n        \"the\",\n        \"board\"\n      ]\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"ISO-639-3 language code\",\n      \"example\": \"eng\"\n    }\n  },\n  \"required\": [\n    \"tokens\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-tokens-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: TokensRequest
---
