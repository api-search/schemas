---
description: SeaTunnel system monitoring information
layout: schema
name: SystemInfo
properties_list:
- description: Number of CPU processors
  name: processors
  type: integer
- description: Total physical memory in bytes
  name: physicalMemory
  type: integer
- description: Free physical memory in bytes
  name: freePhysicalMemory
  type: integer
- description: ''
  name: totalHeapMemory
  type: integer
- description: ''
  name: freeHeapMemory
  type: integer
- description: ''
  name: usedHeapMemory
  type: integer
provider_name: Apache SeaTunnel
provider_slug: apache-seatunnel
schema_file: json-schema/apache-seatunnel-system-info-schema.json
slug: apache-seatunnel-system-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-seatunnel/refs/heads/main/json-schema/apache-seatunnel-system-info-schema.json\",\n  \"title\": \"SystemInfo\",\n  \"description\": \"SeaTunnel system monitoring information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"processors\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of CPU processors\"\n    },\n    \"physicalMemory\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Total physical memory in bytes\"\n    },\n    \"freePhysicalMemory\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Free physical memory in bytes\"\n    },\n    \"totalHeapMemory\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"freeHeapMemory\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"usedHeapMemory\"\
  : {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-seatunnel/refs/heads/main/json-schema/apache-seatunnel-system-info-schema.json
tags:
- Data Integration
- ETL
- ELT
- Batch
- Streaming
- Apache
- Open Source
title: SystemInfo
---
