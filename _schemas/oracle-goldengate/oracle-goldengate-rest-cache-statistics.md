---
description: ''
layout: schema
name: CacheStatistics
properties_list:
- description: ''
  name: processName
  type: string
- description: ''
  name: cacheSize
  type: integer
- description: ''
  name: cacheUsed
  type: integer
- description: ''
  name: cacheHitRatio
  type: number
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-cache-statistics-schema.json
slug: oracle-goldengate-rest-cache-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CacheStatistics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"processName\": {\n      \"type\": \"string\"\n    },\n    \"cacheSize\": {\n      \"type\": \"integer\"\n    },\n    \"cacheUsed\": {\n      \"type\": \"integer\"\n    },\n    \"cacheHitRatio\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-cache-statistics-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: CacheStatistics
---
