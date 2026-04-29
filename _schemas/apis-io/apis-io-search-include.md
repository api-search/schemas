---
description: Include other APIs.json file
layout: schema
name: Include
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: url
  type: string
provider_name: APIs.io
provider_slug: apis-io
schema_file: json-schema/apis-io-search-include-schema.json
slug: apis-io-search-include
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-include-schema.json\",\n  \"title\": \"Include\",\n  \"description\": \"Include other APIs.json file\",\n  \"required\": [\n    \"name\",\n    \"url\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"minLength\": 1\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"pattern\": \"^(http)|(https)://(.*)$\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-include-schema.json
tags:
- API Aggregation
- API Directory
- API Discovery
- API Indexing
- API Rating
- API Search
- APIs.json
- Search Engine
title: Include
---
