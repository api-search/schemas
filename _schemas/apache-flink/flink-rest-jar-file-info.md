---
description: JarFileInfo schema from Apache Flink REST API
layout: schema
name: JarFileInfo
properties_list:
- description: ''
  name: entry
  type: array
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: uploaded
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-jar-file-info-schema.json
slug: flink-rest-jar-file-info
source_filename: flink-rest-jar-file-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-jar-file-info-schema.json\",\n  \"title\": \"JarFileInfo\",\n  \"description\": \"JarFileInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entry\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JarEntryInfo\"\n      }\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"uploaded\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-jar-file-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JarFileInfo
---
