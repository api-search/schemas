---
description: ClusterDataSetListResponseBody schema from Apache Flink REST API
layout: schema
name: ClusterDataSetListResponseBody
properties_list:
- description: ''
  name: dataSets
  type: array
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-cluster-data-set-list-response-body-schema.json
slug: flink-rest-cluster-data-set-list-response-body
source_filename: flink-rest-cluster-data-set-list-response-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-cluster-data-set-list-response-body-schema.json\",\n  \"title\": \"ClusterDataSetListResponseBody\",\n  \"description\": \"ClusterDataSetListResponseBody schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataSets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ClusterDataSetEntry\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-cluster-data-set-list-response-body-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: ClusterDataSetListResponseBody
---
