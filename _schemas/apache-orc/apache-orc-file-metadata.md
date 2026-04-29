---
description: FileMetadata schema from Apache ORC
layout: schema
name: FileMetadata
properties_list:
- description: ''
  name: filePath
  type: string
- description: ''
  name: fileVersion
  type: string
- description: ''
  name: writerVersion
  type: string
- description: ''
  name: compression
  type: string
- description: ''
  name: compressionBlockSize
  type: integer
- description: ''
  name: rowCount
  type: integer
- description: ''
  name: rawDataSize
  type: integer
- description: ''
  name: numberOfStripes
  type: integer
- description: ''
  name: stripes
  type: array
provider_name: Apache ORC
provider_slug: apache-orc
schema_file: json-schema/apache-orc-file-metadata-schema.json
slug: apache-orc-file-metadata
source_filename: apache-orc-file-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-file-metadata-schema.json\",\n  \"title\": \"FileMetadata\",\n  \"description\": \"FileMetadata schema from Apache ORC\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filePath\": {\n      \"type\": \"string\",\n      \"example\": \"data/sales.orc\"\n    },\n    \"fileVersion\": {\n      \"type\": \"string\",\n      \"example\": \"0.12\"\n    },\n    \"writerVersion\": {\n      \"type\": \"string\",\n      \"example\": \"ORC_135\"\n    },\n    \"compression\": {\n      \"type\": \"string\",\n      \"example\": \"ZLIB\",\n      \"enum\": [\n        \"NONE\",\n        \"ZLIB\",\n        \"SNAPPY\",\n        \"LZO\",\n        \"LZ4\",\n        \"ZSTD\"\n      ]\n    },\n    \"compressionBlockSize\": {\n      \"type\": \"integer\",\n      \"example\": 262144\n    },\n    \"rowCount\": {\n    \
  \  \"type\": \"integer\",\n      \"example\": 1000000\n    },\n    \"rawDataSize\": {\n      \"type\": \"integer\",\n      \"example\": 104857600\n    },\n    \"numberOfStripes\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"stripes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StripeInfo\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-file-metadata-schema.json
tags:
- Big Data
- Columnar Storage
- Compression
- File Format
- Hadoop
- Apache
- Open Source
title: FileMetadata
---
