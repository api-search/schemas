---
description: MediaList schema from Instagram Graph API
layout: schema
name: MediaList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: paging
  type: object
provider_name: Instagram
provider_slug: instagram
schema_file: json-schema/instagram-graph-api-media-list-schema.json
slug: instagram-graph-api-media-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/json-schema/instagram-graph-api-media-list-schema.json\",\n  \"title\": \"MediaList\",\n  \"description\": \"MediaList schema from Instagram Graph API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Media\"\n      }\n    },\n    \"paging\": {\n      \"$ref\": \"#/components/schemas/Paging\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/json-schema/instagram-graph-api-media-list-schema.json
tags:
- Instagram
- Meta
- Photos
- Social Media
- Videos
- Content Publishing
title: MediaList
---
