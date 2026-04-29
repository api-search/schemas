---
description: TableList schema from Apache Pinot
layout: schema
name: TableList
properties_list:
- description: ''
  name: tables
  type: array
provider_name: Apache Pinot
provider_slug: apache-pinot
schema_file: json-schema/apache-pinot-table-list-schema.json
slug: apache-pinot-table-list
source_filename: apache-pinot-table-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-table-list-schema.json\",\n  \"title\": \"TableList\",\n  \"description\": \"TableList schema from Apache Pinot\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tables\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"airlineStats_OFFLINE\",\n        \"baseballStats_OFFLINE\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-table-list-schema.json
tags:
- Analytics
- Database
- Low Latency
- OLAP
- Real-Time
- Apache
- Open Source
title: TableList
---
