---
description: MergeRequest schema from Apache ORC
layout: schema
name: MergeRequest
properties_list:
- description: ''
  name: inputPaths
  type: array
- description: ''
  name: outputPath
  type: string
provider_name: Apache ORC
provider_slug: apache-orc
schema_file: json-schema/apache-orc-merge-request-schema.json
slug: apache-orc-merge-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-merge-request-schema.json\",\n  \"title\": \"MergeRequest\",\n  \"description\": \"MergeRequest schema from Apache ORC\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputPaths\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"data/part-001.orc\",\n        \"data/part-002.orc\"\n      ]\n    },\n    \"outputPath\": {\n      \"type\": \"string\",\n      \"example\": \"data/merged.orc\"\n    }\n  },\n  \"required\": [\n    \"inputPaths\",\n    \"outputPath\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-merge-request-schema.json
tags:
- Big Data
- Columnar Storage
- Compression
- File Format
- Hadoop
- Apache
- Open Source
title: MergeRequest
---
