---
description: Link schema from APIs.io Search API
layout: schema
name: Link
properties_list:
- description: ''
  name: self
  type: string
- description: ''
  name: first
  type: string
- description: ''
  name: prev
  type: string
- description: ''
  name: next
  type: string
- description: ''
  name: last
  type: string
provider_name: APIs.io
provider_slug: apis-io
schema_file: json-schema/apis-io-search-link-schema.json
slug: apis-io-search-link
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-link-schema.json\",\n  \"title\": \"Link\",\n  \"description\": \"Link schema from APIs.io Search API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\"\n    },\n    \"first\": {\n      \"type\": \"string\"\n    },\n    \"prev\": {\n      \"type\": \"string\"\n    },\n    \"next\": {\n      \"type\": \"string\"\n    },\n    \"last\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"self\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-link-schema.json
tags:
- API Aggregation
- API Directory
- API Discovery
- API Indexing
- API Rating
- API Search
- APIs.json
- Search Engine
title: Link
---
