---
description: A single collocation result returned by the Linguatools Collocations API.
layout: schema
name: Linguatools Collocation
properties_list:
- description: The base query word.
  name: basis
  type: string
- description: The collocated word or phrase.
  name: collocate
  type: string
- description: Syntactic relation between the basis and the collocate, such as V:obj:N or N:mod:Adj.
  name: relation
  type: string
- description: Statistical significance score of the collocation.
  name: significance
  type: number
- description: Up to three example sentences for the collocation.
  name: examples
  type: array
provider_name: Linguatools
provider_slug: linguatools
schema_file: json-schema/linguatools-collocation-schema.json
slug: linguatools-collocation
source_filename: linguatools-collocation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linguatools/refs/heads/main/json-schema/linguatools-collocation-schema.json\",\n  \"title\": \"Linguatools Collocation\",\n  \"description\": \"A single collocation result returned by the Linguatools Collocations API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"basis\": {\n      \"type\": \"string\",\n      \"description\": \"The base query word.\"\n    },\n    \"collocate\": {\n      \"type\": \"string\",\n      \"description\": \"The collocated word or phrase.\"\n    },\n    \"relation\": {\n      \"type\": \"string\",\n      \"description\": \"Syntactic relation between the basis and the collocate, such as V:obj:N or N:mod:Adj.\"\n    },\n    \"significance\": {\n      \"type\": \"number\",\n      \"description\": \"Statistical significance score of the collocation.\"\n    },\n    \"examples\": {\n      \"type\": \"array\",\n    \
  \  \"description\": \"Up to three example sentences for the collocation.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"maxItems\": 3\n    }\n  },\n  \"required\": [\"basis\", \"collocate\", \"relation\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linguatools/refs/heads/main/json-schema/linguatools-collocation-schema.json
tags:
- Collocations
- Dictionary
- English
- Language
- Linguistics
- NLP
title: Linguatools Collocation
---
