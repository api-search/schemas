---
description: Paging schema from Instagram Graph API
layout: schema
name: Paging
properties_list:
- description: ''
  name: cursors
  type: object
- description: URL to fetch next page.
  name: next
  type: string
- description: URL to fetch previous page.
  name: previous
  type: string
provider_name: Instagram
provider_slug: instagram
schema_file: json-schema/instagram-graph-api-paging-schema.json
slug: instagram-graph-api-paging
source_filename: instagram-graph-api-paging-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/json-schema/instagram-graph-api-paging-schema.json\",\n  \"title\": \"Paging\",\n  \"description\": \"Paging schema from Instagram Graph API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cursors\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"before\": {\n          \"type\": \"string\",\n          \"example\": \"QVFIUjRtc2c5NEl0ajN3\"\n        },\n        \"after\": {\n          \"type\": \"string\",\n          \"example\": \"QVFIUmlKdXBzYWtyUml3\"\n        }\n      }\n    },\n    \"next\": {\n      \"type\": \"string\",\n      \"description\": \"URL to fetch next page.\"\n    },\n    \"previous\": {\n      \"type\": \"string\",\n      \"description\": \"URL to fetch previous page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/json-schema/instagram-graph-api-paging-schema.json
tags:
- Instagram
- Meta
- Photos
- Social Media
- Videos
- Content Publishing
title: Paging
---
