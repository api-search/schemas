---
description: ResultTable schema from Apache Pinot
layout: schema
name: ResultTable
properties_list:
- description: ''
  name: dataSchema
  type: object
- description: ''
  name: rows
  type: array
provider_name: Apache Pinot
provider_slug: apache-pinot
schema_file: json-schema/apache-pinot-result-table-schema.json
slug: apache-pinot-result-table
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-result-table-schema.json\",\n  \"title\": \"ResultTable\",\n  \"description\": \"ResultTable schema from Apache Pinot\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataSchema\": {\n      \"$ref\": \"#/components/schemas/DataSchema\"\n    },\n    \"rows\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {}\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-result-table-schema.json
tags:
- Analytics
- Database
- Low Latency
- OLAP
- Real-Time
- Apache
- Open Source
title: ResultTable
---
