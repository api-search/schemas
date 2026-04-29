---
description: Meta schema from APIs.io Search API
layout: schema
name: Meta
properties_list:
- description: ''
  name: search
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: limit
  type: integer
- description: ''
  name: page
  type: integer
- description: ''
  name: totalPages
  type: integer
provider_name: APIs.io
provider_slug: apis-io
schema_file: json-schema/apis-io-search-meta-schema.json
slug: apis-io-search-meta
source_filename: apis-io-search-meta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-meta-schema.json\",\n  \"title\": \"Meta\",\n  \"description\": \"Meta schema from APIs.io Search API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"search\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"page\": {\n      \"type\": \"integer\"\n    },\n    \"totalPages\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"totalPages\",\n    \"page\",\n    \"limit\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-meta-schema.json
tags:
- API Aggregation
- API Directory
- API Discovery
- API Indexing
- API Rating
- API Search
- APIs.json
- Search Engine
title: Meta
---
