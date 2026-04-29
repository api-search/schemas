---
description: Hudi query configuration for incremental or snapshot queries
layout: schema
name: QueryConfig
properties_list:
- description: Query type (SNAPSHOT, INCREMENTAL, READ_OPTIMIZED)
  name: queryType
  type: string
- description: Start instant for incremental queries
  name: beginInstantTime
  type: string
- description: End instant for incremental queries
  name: endInstantTime
  type: string
- description: Maximum commits to include in incremental query
  name: maxCommits
  type: integer
provider_name: Apache Hudi
provider_slug: apache-hudi
schema_file: json-schema/hudi-queryconfig-schema.json
slug: hudi-queryconfig
source_filename: hudi-queryconfig-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hudi/json-schema/hudi-queryconfig-schema.json\",\n  \"title\": \"QueryConfig\",\n  \"type\": \"object\",\n  \"description\": \"Hudi query configuration for incremental or snapshot queries\",\n  \"properties\": {\n    \"queryType\": {\n      \"type\": \"string\",\n      \"description\": \"Query type (SNAPSHOT, INCREMENTAL, READ_OPTIMIZED)\",\n      \"example\": \"SNAPSHOT\"\n    },\n    \"beginInstantTime\": {\n      \"type\": \"string\",\n      \"description\": \"Start instant for incremental queries\",\n      \"example\": \"20240101000000000\"\n    },\n    \"endInstantTime\": {\n      \"type\": \"string\",\n      \"description\": \"End instant for incremental queries\",\n      \"example\": \"20240101120000000\"\n    },\n    \"maxCommits\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum commits to include in incremental query\",\n      \"example\"\
  : 10\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hudi/refs/heads/main/json-schema/hudi-queryconfig-schema.json
tags:
- ACID
- Apache
- Big Data
- Data Lake
- Incremental Processing
- Lakehouse
- Open Source
title: QueryConfig
---
