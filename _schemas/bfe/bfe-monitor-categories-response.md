---
description: List of available monitor metric categories.
layout: schema
name: MonitorCategoriesResponse
properties_list:
- description: Available monitor category names.
  name: categories
  type: array
provider_name: BFE
provider_slug: bfe
schema_file: json-schema/bfe-monitor-categories-response-schema.json
slug: bfe-monitor-categories-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bfe/refs/heads/main/json-schema/bfe-monitor-categories-response-schema.json\",\n  \"title\": \"MonitorCategoriesResponse\",\n  \"description\": \"List of available monitor metric categories.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"categories\": {\n      \"type\": \"array\",\n      \"description\": \"Available monitor category names.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"connections\",\n        \"requests\",\n        \"routing\",\n        \"upstream\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bfe/refs/heads/main/json-schema/bfe-monitor-categories-response-schema.json
tags:
- Load Balancer
- Networking
- Open Source
- Traffic Management
- CNCF
- Baidu
title: MonitorCategoriesResponse
---
