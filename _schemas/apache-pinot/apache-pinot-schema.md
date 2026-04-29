---
description: Schema schema from Apache Pinot
layout: schema
name: Schema
properties_list:
- description: ''
  name: schemaName
  type: string
- description: ''
  name: dimensionFieldSpecs
  type: array
- description: ''
  name: metricFieldSpecs
  type: array
- description: ''
  name: dateTimeFieldSpecs
  type: array
provider_name: Apache Pinot
provider_slug: apache-pinot
schema_file: json-schema/apache-pinot-schema-schema.json
slug: apache-pinot-schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-schema-schema.json\",\n  \"title\": \"Schema\",\n  \"description\": \"Schema schema from Apache Pinot\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemaName\": {\n      \"type\": \"string\",\n      \"example\": \"airlineStats\"\n    },\n    \"dimensionFieldSpecs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FieldSpec\"\n      }\n    },\n    \"metricFieldSpecs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FieldSpec\"\n      }\n    },\n    \"dateTimeFieldSpecs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FieldSpec\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-schema-schema.json
tags:
- Analytics
- Database
- Low Latency
- OLAP
- Real-Time
- Apache
- Open Source
title: Schema
---
