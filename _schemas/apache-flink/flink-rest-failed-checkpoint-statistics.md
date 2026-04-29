---
description: FailedCheckpointStatistics schema from Apache Flink REST API
layout: schema
name: FailedCheckpointStatistics
properties_list: []
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-failed-checkpoint-statistics-schema.json
slug: flink-rest-failed-checkpoint-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-failed-checkpoint-statistics-schema.json\",\n  \"title\": \"FailedCheckpointStatistics\",\n  \"description\": \"FailedCheckpointStatistics schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/CheckpointStatistics\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"failure_timestamp\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"failure_message\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-failed-checkpoint-statistics-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: FailedCheckpointStatistics
---
