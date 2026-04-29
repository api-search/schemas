---
description: ExecutionState schema from Apache Flink REST API
layout: schema
name: ExecutionState
properties_list: []
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-execution-state-schema.json
slug: flink-rest-execution-state
source_filename: flink-rest-execution-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-execution-state-schema.json\",\n  \"title\": \"ExecutionState\",\n  \"description\": \"ExecutionState schema from Apache Flink REST API\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"CREATED\",\n    \"SCHEDULED\",\n    \"DEPLOYING\",\n    \"RUNNING\",\n    \"FINISHED\",\n    \"CANCELING\",\n    \"CANCELED\",\n    \"FAILED\",\n    \"RECONCILING\",\n    \"INITIALIZING\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-execution-state-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: ExecutionState
---
