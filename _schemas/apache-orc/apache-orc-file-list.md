---
description: FileList schema from Apache ORC
layout: schema
name: FileList
properties_list:
- description: ''
  name: files
  type: array
provider_name: Apache ORC
provider_slug: apache-orc
schema_file: json-schema/apache-orc-file-list-schema.json
slug: apache-orc-file-list
source_filename: apache-orc-file-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-file-list-schema.json\",\n  \"title\": \"FileList\",\n  \"description\": \"FileList schema from Apache ORC\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"files\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FileInfo\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-file-list-schema.json
tags:
- Big Data
- Columnar Storage
- Compression
- File Format
- Hadoop
- Apache
- Open Source
title: FileList
---
