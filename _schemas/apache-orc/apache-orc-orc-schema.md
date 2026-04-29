---
description: OrcSchema schema from Apache ORC
layout: schema
name: OrcSchema
properties_list:
- description: Top-level type name
  name: typeName
  type: string
- description: ''
  name: columns
  type: array
provider_name: Apache ORC
provider_slug: apache-orc
schema_file: json-schema/apache-orc-orc-schema-schema.json
slug: apache-orc-orc-schema
source_filename: apache-orc-orc-schema-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-orc-schema-schema.json\",\n  \"title\": \"OrcSchema\",\n  \"description\": \"OrcSchema schema from Apache ORC\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"typeName\": {\n      \"type\": \"string\",\n      \"description\": \"Top-level type name\",\n      \"example\": \"struct\"\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ColumnType\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-orc-schema-schema.json
tags:
- Big Data
- Columnar Storage
- Compression
- File Format
- Hadoop
- Apache
- Open Source
title: OrcSchema
---
