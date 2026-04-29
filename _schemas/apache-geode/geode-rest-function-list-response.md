---
description: Response containing list of available functions
layout: schema
name: FunctionListResponse
properties_list:
- description: List of function IDs
  name: functions
  type: array
provider_name: Apache Geode
provider_slug: apache-geode
schema_file: json-schema/geode-rest-function-list-response-schema.json
slug: geode-rest-function-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-function-list-response-schema.json\",\n  \"title\": \"FunctionListResponse\",\n  \"description\": \"Response containing list of available functions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"functions\": {\n      \"type\": \"array\",\n      \"description\": \"List of function IDs\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"calculateTotals\",\n        \"cleanupExpired\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-function-list-response-schema.json
tags:
- Apache
- Caching
- Data Grid
- Distributed Systems
- In-Memory
- Open Source
title: FunctionListResponse
---
