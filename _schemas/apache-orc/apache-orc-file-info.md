---
description: FileInfo schema from Apache ORC
layout: schema
name: FileInfo
properties_list:
- description: ''
  name: path
  type: string
- description: File size in bytes
  name: size
  type: integer
- description: ''
  name: rowCount
  type: integer
- description: ''
  name: stripes
  type: integer
provider_name: Apache ORC
provider_slug: apache-orc
schema_file: json-schema/apache-orc-file-info-schema.json
slug: apache-orc-file-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-file-info-schema.json\",\n  \"title\": \"FileInfo\",\n  \"description\": \"FileInfo schema from Apache ORC\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\",\n      \"example\": \"data/sales.orc\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"File size in bytes\",\n      \"example\": 10485760\n    },\n    \"rowCount\": {\n      \"type\": \"integer\",\n      \"example\": 1000000\n    },\n    \"stripes\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-file-info-schema.json
tags:
- Big Data
- Columnar Storage
- Compression
- File Format
- Hadoop
- Apache
- Open Source
title: FileInfo
---
