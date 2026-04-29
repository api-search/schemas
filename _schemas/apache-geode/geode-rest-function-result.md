---
description: Results from function execution
layout: schema
name: FunctionResult
properties_list:
- description: Function return values
  name: result
  type: array
provider_name: Apache Geode
provider_slug: apache-geode
schema_file: json-schema/geode-rest-function-result-schema.json
slug: geode-rest-function-result
source_filename: geode-rest-function-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-function-result-schema.json\",\n  \"title\": \"FunctionResult\",\n  \"description\": \"Results from function execution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"result\": {\n      \"type\": \"array\",\n      \"description\": \"Function return values\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-function-result-schema.json
tags:
- Apache
- Caching
- Data Grid
- Distributed Systems
- In-Memory
- Open Source
title: FunctionResult
---
