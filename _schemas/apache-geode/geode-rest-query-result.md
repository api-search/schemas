---
description: Results from an OQL query execution
layout: schema
name: QueryResult
properties_list:
- description: Query result objects
  name: result
  type: array
provider_name: Apache Geode
provider_slug: apache-geode
schema_file: json-schema/geode-rest-query-result-schema.json
slug: geode-rest-query-result
source_filename: geode-rest-query-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-query-result-schema.json\",\n  \"title\": \"QueryResult\",\n  \"description\": \"Results from an OQL query execution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"result\": {\n      \"type\": \"array\",\n      \"description\": \"Query result objects\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-query-result-schema.json
tags:
- Apache
- Caching
- Data Grid
- Distributed Systems
- In-Memory
- Open Source
title: QueryResult
---
