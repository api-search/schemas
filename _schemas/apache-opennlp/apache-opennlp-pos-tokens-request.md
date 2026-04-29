---
description: POSTokensRequest schema from Apache OpenNLP
layout: schema
name: POSTokensRequest
properties_list:
- description: Pre-tokenized array of text tokens
  name: tokens
  type: array
- description: POS tags for each token
  name: posTags
  type: array
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-pos-tokens-request-schema.json
slug: apache-opennlp-pos-tokens-request
source_filename: apache-opennlp-pos-tokens-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-pos-tokens-request-schema.json\",\n  \"title\": \"POSTokensRequest\",\n  \"description\": \"POSTokensRequest schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tokens\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Pre-tokenized array of text tokens\",\n      \"example\": [\n        \"Pierre\",\n        \"Vinken\",\n        \"will\",\n        \"join\"\n      ]\n    },\n    \"posTags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"POS tags for each token\",\n      \"example\": [\n        \"NNP\",\n        \"NNP\",\n        \"MD\",\n        \"VB\"\n      ]\n    }\n  },\n  \"required\": [\n    \"tokens\",\n    \"posTags\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-pos-tokens-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: POSTokensRequest
---
