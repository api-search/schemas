---
description: ConversionRequest schema from Apache ORC
layout: schema
name: ConversionRequest
properties_list:
- description: ''
  name: sourcePath
  type: string
- description: ''
  name: outputPath
  type: string
- description: ''
  name: sourceFormat
  type: string
- description: ''
  name: compression
  type: string
- description: ''
  name: rowBatchSize
  type: integer
provider_name: Apache ORC
provider_slug: apache-orc
schema_file: json-schema/apache-orc-conversion-request-schema.json
slug: apache-orc-conversion-request
source_filename: apache-orc-conversion-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-conversion-request-schema.json\",\n  \"title\": \"ConversionRequest\",\n  \"description\": \"ConversionRequest schema from Apache ORC\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourcePath\": {\n      \"type\": \"string\",\n      \"example\": \"data/sales.csv\"\n    },\n    \"outputPath\": {\n      \"type\": \"string\",\n      \"example\": \"data/sales.orc\"\n    },\n    \"sourceFormat\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"csv\",\n        \"json\",\n        \"parquet\",\n        \"avro\"\n      ],\n      \"example\": \"csv\"\n    },\n    \"compression\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"NONE\",\n        \"ZLIB\",\n        \"SNAPPY\",\n        \"LZ4\",\n        \"ZSTD\"\n      ],\n      \"example\": \"ZLIB\"\n    },\n    \"rowBatchSize\"\
  : {\n      \"type\": \"integer\",\n      \"example\": 1024\n    }\n  },\n  \"required\": [\n    \"sourcePath\",\n    \"outputPath\",\n    \"sourceFormat\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-conversion-request-schema.json
tags:
- Big Data
- Columnar Storage
- Compression
- File Format
- Hadoop
- Apache
- Open Source
title: ConversionRequest
---
