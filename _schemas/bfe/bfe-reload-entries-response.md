---
description: List of available configuration reload entries.
layout: schema
name: ReloadEntriesResponse
properties_list:
- description: Available reload entry names.
  name: entries
  type: array
provider_name: BFE
provider_slug: bfe
schema_file: json-schema/bfe-reload-entries-response-schema.json
slug: bfe-reload-entries-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bfe/refs/heads/main/json-schema/bfe-reload-entries-response-schema.json\",\n  \"title\": \"ReloadEntriesResponse\",\n  \"description\": \"List of available configuration reload entries.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entries\": {\n      \"type\": \"array\",\n      \"description\": \"Available reload entry names.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ReloadEntry\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bfe/refs/heads/main/json-schema/bfe-reload-entries-response-schema.json
tags:
- Load Balancer
- Networking
- Open Source
- Traffic Management
- CNCF
- Baidu
title: ReloadEntriesResponse
---
