---
description: HardwareDescription schema from Apache Flink REST API
layout: schema
name: HardwareDescription
properties_list:
- description: ''
  name: cpuCores
  type: integer
- description: ''
  name: freeMemory
  type: integer
- description: ''
  name: managedMemory
  type: integer
- description: ''
  name: physicalMemory
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-hardware-description-schema.json
slug: flink-rest-hardware-description
source_filename: flink-rest-hardware-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-hardware-description-schema.json\",\n  \"title\": \"HardwareDescription\",\n  \"description\": \"HardwareDescription schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cpuCores\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"freeMemory\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"managedMemory\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"physicalMemory\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-hardware-description-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: HardwareDescription
---
