---
description: JobStatus schema from Apache Flink REST API
layout: schema
name: JobStatus
properties_list: []
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-job-status-schema.json
slug: flink-rest-job-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-status-schema.json\",\n  \"title\": \"JobStatus\",\n  \"description\": \"JobStatus schema from Apache Flink REST API\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"INITIALIZING\",\n    \"CREATED\",\n    \"RUNNING\",\n    \"FAILING\",\n    \"FAILED\",\n    \"CANCELLING\",\n    \"CANCELED\",\n    \"FINISHED\",\n    \"RESTARTING\",\n    \"SUSPENDED\",\n    \"RECONCILING\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-status-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JobStatus
---
