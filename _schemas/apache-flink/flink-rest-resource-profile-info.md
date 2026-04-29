---
description: ResourceProfileInfo schema from Apache Flink REST API
layout: schema
name: ResourceProfileInfo
properties_list:
- description: ''
  name: cpuCores
  type: number
- description: ''
  name: extendedResources
  type: object
- description: ''
  name: managedMemory
  type: integer
- description: ''
  name: networkMemory
  type: integer
- description: ''
  name: taskHeapMemory
  type: integer
- description: ''
  name: taskOffHeapMemory
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-resource-profile-info-schema.json
slug: flink-rest-resource-profile-info
source_filename: flink-rest-resource-profile-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-resource-profile-info-schema.json\",\n  \"title\": \"ResourceProfileInfo\",\n  \"description\": \"ResourceProfileInfo schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cpuCores\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"extendedResources\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"number\",\n        \"format\": \"double\"\n      }\n    },\n    \"managedMemory\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"networkMemory\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"taskHeapMemory\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"taskOffHeapMemory\": {\n      \"type\": \"integer\",\n\
  \      \"format\": \"int32\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-resource-profile-info-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: ResourceProfileInfo
---
