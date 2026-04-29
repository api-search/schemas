---
description: Named OQL query metadata
layout: schema
name: QueryInfo
properties_list:
- description: Unique query identifier
  name: id
  type: string
- description: OQL query string
  name: oql
  type: string
provider_name: Apache Geode
provider_slug: apache-geode
schema_file: json-schema/geode-rest-query-info-schema.json
slug: geode-rest-query-info
source_filename: geode-rest-query-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-query-info-schema.json\",\n  \"title\": \"QueryInfo\",\n  \"description\": \"Named OQL query metadata\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique query identifier\",\n      \"example\": \"getPendingOrders\"\n    },\n    \"oql\": {\n      \"type\": \"string\",\n      \"description\": \"OQL query string\",\n      \"example\": \"SELECT * FROM /orders WHERE status='PENDING'\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-query-info-schema.json
tags:
- Apache
- Caching
- Data Grid
- Distributed Systems
- In-Memory
- Open Source
title: QueryInfo
---
