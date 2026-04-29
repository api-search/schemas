---
description: LatestCheckpoints schema from Apache Flink REST API
layout: schema
name: LatestCheckpoints
properties_list:
- description: ''
  name: completed
  type: object
- description: ''
  name: failed
  type: object
- description: ''
  name: restored
  type: object
- description: ''
  name: savepoint
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-latest-checkpoints-schema.json
slug: flink-rest-latest-checkpoints
source_filename: flink-rest-latest-checkpoints-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-latest-checkpoints-schema.json\",\n  \"title\": \"LatestCheckpoints\",\n  \"description\": \"LatestCheckpoints schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"completed\": {\n      \"$ref\": \"#/components/schemas/CompletedCheckpointStatistics\"\n    },\n    \"failed\": {\n      \"$ref\": \"#/components/schemas/FailedCheckpointStatistics\"\n    },\n    \"restored\": {\n      \"$ref\": \"#/components/schemas/RestoredCheckpointStatistics\"\n    },\n    \"savepoint\": {\n      \"$ref\": \"#/components/schemas/CompletedCheckpointStatistics\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-latest-checkpoints-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: LatestCheckpoints
---
