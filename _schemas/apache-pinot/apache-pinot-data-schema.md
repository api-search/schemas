---
description: DataSchema schema from Apache Pinot
layout: schema
name: DataSchema
properties_list:
- description: ''
  name: columnNames
  type: array
- description: ''
  name: columnDataTypes
  type: array
provider_name: Apache Pinot
provider_slug: apache-pinot
schema_file: json-schema/apache-pinot-data-schema-schema.json
slug: apache-pinot-data-schema
source_filename: apache-pinot-data-schema-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-data-schema-schema.json\",\n  \"title\": \"DataSchema\",\n  \"description\": \"DataSchema schema from Apache Pinot\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"columnNames\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"count(*)\"\n      ]\n    },\n    \"columnDataTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"LONG\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-data-schema-schema.json
tags:
- Analytics
- Database
- Low Latency
- OLAP
- Real-Time
- Apache
- Open Source
title: DataSchema
---
