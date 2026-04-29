---
description: OperationResult schema from Apache ORC
layout: schema
name: OperationResult
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
provider_name: Apache ORC
provider_slug: apache-orc
schema_file: json-schema/apache-orc-operation-result-schema.json
slug: apache-orc-operation-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-operation-result-schema.json\",\n  \"title\": \"OperationResult\",\n  \"description\": \"OperationResult schema from Apache ORC\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"success\",\n        \"failure\"\n      ],\n      \"example\": \"success\"\n    },\n    \"outputPath\": {\n      \"type\": \"string\",\n      \"example\": \"data/merged.orc\"\n    },\n    \"rowsWritten\": {\n      \"type\": \"integer\",\n      \"example\": 2000000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-operation-result-schema.json
tags:
- Big Data
- Columnar Storage
- Compression
- File Format
- Hadoop
- Apache
- Open Source
title: OperationResult
---
