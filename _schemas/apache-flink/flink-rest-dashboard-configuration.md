---
description: DashboardConfiguration schema from Apache Flink REST API
layout: schema
name: DashboardConfiguration
properties_list:
- description: ''
  name: features
  type: object
- description: ''
  name: flink-revision
  type: string
- description: ''
  name: flink-version
  type: string
- description: ''
  name: refresh-interval
  type: integer
- description: ''
  name: timezone-name
  type: string
- description: ''
  name: timezone-offset
  type: integer
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-dashboard-configuration-schema.json
slug: flink-rest-dashboard-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-dashboard-configuration-schema.json\",\n  \"title\": \"DashboardConfiguration\",\n  \"description\": \"DashboardConfiguration schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"features\": {\n      \"$ref\": \"#/components/schemas/Features\"\n    },\n    \"flink-revision\": {\n      \"type\": \"string\"\n    },\n    \"flink-version\": {\n      \"type\": \"string\"\n    },\n    \"refresh-interval\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"timezone-name\": {\n      \"type\": \"string\"\n    },\n    \"timezone-offset\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-dashboard-configuration-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: DashboardConfiguration
---
