---
description: MetricCollectionResponseBody schema from Apache Flink REST API
layout: schema
name: MetricCollectionResponseBody
properties_list:
- description: ''
  name: metrics
  type: array
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-metric-collection-response-body-schema.json
slug: flink-rest-metric-collection-response-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-metric-collection-response-body-schema.json\",\n  \"title\": \"MetricCollectionResponseBody\",\n  \"description\": \"MetricCollectionResponseBody schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metrics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Metric\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-metric-collection-response-body-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: MetricCollectionResponseBody
---
