---
description: Response containing list of saved OQL queries
layout: schema
name: QueryListResponse
properties_list:
- description: List of saved queries
  name: queries
  type: array
provider_name: Apache Geode
provider_slug: apache-geode
schema_file: json-schema/geode-rest-query-list-response-schema.json
slug: geode-rest-query-list-response
source_filename: geode-rest-query-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-query-list-response-schema.json\",\n  \"title\": \"QueryListResponse\",\n  \"description\": \"Response containing list of saved OQL queries\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queries\": {\n      \"type\": \"array\",\n      \"description\": \"List of saved queries\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/QueryInfo\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-query-list-response-schema.json
tags:
- Apache
- Caching
- Data Grid
- Distributed Systems
- In-Memory
- Open Source
title: QueryListResponse
---
