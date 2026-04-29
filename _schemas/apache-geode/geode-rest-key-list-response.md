---
description: Response containing all keys in a region
layout: schema
name: KeyListResponse
properties_list:
- description: List of region keys
  name: keys
  type: array
provider_name: Apache Geode
provider_slug: apache-geode
schema_file: json-schema/geode-rest-key-list-response-schema.json
slug: geode-rest-key-list-response
source_filename: geode-rest-key-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-key-list-response-schema.json\",\n  \"title\": \"KeyListResponse\",\n  \"description\": \"Response containing all keys in a region\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keys\": {\n      \"type\": \"array\",\n      \"description\": \"List of region keys\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"order-001\",\n        \"order-002\",\n        \"order-003\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-key-list-response-schema.json
tags:
- Apache
- Caching
- Data Grid
- Distributed Systems
- In-Memory
- Open Source
title: KeyListResponse
---
