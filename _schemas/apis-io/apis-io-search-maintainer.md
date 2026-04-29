---
description: The person or organization responsible for maintaining the API.
layout: schema
name: Maintainer
properties_list:
- description: name
  name: name
  type: string
provider_name: APIs.io
provider_slug: apis-io
schema_file: json-schema/apis-io-search-maintainer-schema.json
slug: apis-io-search-maintainer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-maintainer-schema.json\",\n  \"title\": \"Maintainer\",\n  \"description\": \"The person or organization responsible for maintaining the API.\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"name\",\n      \"minLength\": 5\n    }\n  },\n  \"additionalProperties\": {\n    \"type\": \"string\"\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-maintainer-schema.json
tags:
- API Aggregation
- API Directory
- API Discovery
- API Indexing
- API Rating
- API Search
- APIs.json
- Search Engine
title: Maintainer
---
