---
description: ClusterOverviewWithVersion schema from Apache Flink REST API
layout: schema
name: ClusterOverviewWithVersion
properties_list:
- description: ''
  name: flink-commit
  type: string
- description: ''
  name: flink-version
  type: string
- description: ''
  name: jobs-cancelled
  type: integer
- description: ''
  name: jobs-failed
  type: integer
- description: ''
  name: jobs-finished
  type: integer
- description: ''
  name: jobs-running
  type: integer
- description: ''
  name: slots-available
  type: integer
- description: ''
  name: slots-free-and-blocked
  type: integer
- description: ''
  name: slots-total
  type: integer
- description: ''
  name: taskmanagers
  type: integer
- description: ''
  name: taskmanagers-blocked
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-cluster-overview-with-version-schema.json
slug: flink-rest-cluster-overview-with-version
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-cluster-overview-with-version-schema.json\",\n  \"title\": \"ClusterOverviewWithVersion\",\n  \"description\": \"ClusterOverviewWithVersion schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flink-commit\": {\n      \"type\": \"string\"\n    },\n    \"flink-version\": {\n      \"type\": \"string\"\n    },\n    \"jobs-cancelled\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"jobs-failed\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"jobs-finished\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"jobs-running\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"slots-available\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n\
  \    },\n    \"slots-free-and-blocked\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"slots-total\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"taskmanagers\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"taskmanagers-blocked\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-cluster-overview-with-version-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: ClusterOverviewWithVersion
---
