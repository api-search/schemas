---
description: An JSON API object with metadata, data, and links.
layout: schema
name: Search
properties_list:
- description: ''
  name: meta
  type: object
- description: ''
  name: data
  type: object
- description: ''
  name: links
  type: object
provider_name: APIs.io
provider_slug: apis-io
schema_file: json-schema/apis-io-search-search-schema.json
slug: apis-io-search-search
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-search-schema.json\",\n  \"title\": \"Search\",\n  \"description\": \"An JSON API object with metadata, data, and links.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"meta\": {\n      \"$ref\": \"#/components/schemas/Meta\"\n    },\n    \"data\": {\n      \"$ref\": \"#/components/schemas/APIs\"\n    },\n    \"links\": {\n      \"$ref\": \"#/components/schemas/Link\"\n    }\n  },\n  \"required\": [\n    \"meta\",\n    \"data\",\n    \"links\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-search-schema.json
tags:
- API Aggregation
- API Directory
- API Discovery
- API Indexing
- API Rating
- API Search
- APIs.json
- Search Engine
title: Search
---
