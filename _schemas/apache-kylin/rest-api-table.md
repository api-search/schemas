---
description: A Kylin table
layout: schema
name: Table
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: columns
  type: array
- description: ''
  name: cardinality
  type: object
- description: ''
  name: exd
  type: object
provider_name: Apache Kylin
provider_slug: apache-kylin
schema_file: json-schema/rest-api-table-schema.json
slug: rest-api-table
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/json-schema/rest-api-table-schema.json\",\n  \"title\": \"Table\",\n  \"description\": \"A Kylin table\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"KYLIN_SALES\"\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"cardinality\": {\n      \"type\": \"object\"\n    },\n    \"exd\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/json-schema/rest-api-table-schema.json
tags:
- Analytics
- Big Data
- Cube
- OLAP
- Open Source
- SQL
title: Table
---
