---
description: ConversionResult schema from Apache ORC
layout: schema
name: ConversionResult
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: outputPath
  type: string
- description: ''
  name: rowsWritten
  type: integer
- description: Duration in milliseconds
  name: duration
  type: integer
provider_name: Apache ORC
provider_slug: apache-orc
schema_file: json-schema/apache-orc-conversion-result-schema.json
slug: apache-orc-conversion-result
source_filename: apache-orc-conversion-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-conversion-result-schema.json\",\n  \"title\": \"ConversionResult\",\n  \"description\": \"ConversionResult schema from Apache ORC\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"success\",\n        \"failure\"\n      ],\n      \"example\": \"success\"\n    },\n    \"outputPath\": {\n      \"type\": \"string\",\n      \"example\": \"data/sales.orc\"\n    },\n    \"rowsWritten\": {\n      \"type\": \"integer\",\n      \"example\": 1000000\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration in milliseconds\",\n      \"example\": 5234\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-conversion-result-schema.json
tags:
- Big Data
- Columnar Storage
- Compression
- File Format
- Hadoop
- Apache
- Open Source
title: ConversionResult
---
