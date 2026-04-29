---
description: AddAPIsJSON schema from APIs.io Search API
layout: schema
name: AddAPIsJSON
properties_list:
- description: URL where the apis.json file will live
  name: url
  type: string
provider_name: APIs.io
provider_slug: apis-io
schema_file: json-schema/apis-io-search-add-ap-is-json-schema.json
slug: apis-io-search-add-ap-is-json
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-add-ap-is-json-schema.json\",\n  \"title\": \"AddAPIsJSON\",\n  \"description\": \"AddAPIsJSON schema from APIs.io Search API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"url\"\n  ],\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"URL where the apis.json file will live\",\n      \"pattern\": \"^(http)|(https)://(.*)$\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-add-ap-is-json-schema.json
tags:
- API Aggregation
- API Directory
- API Discovery
- API Indexing
- API Rating
- API Search
- APIs.json
- Search Engine
title: AddAPIsJSON
---
