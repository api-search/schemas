---
description: JobIdsWithStatusOverview schema from Apache Flink REST API
layout: schema
name: JobIdsWithStatusOverview
properties_list:
- description: ''
  name: jobs
  type: array
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-job-ids-with-status-overview-schema.json
slug: flink-rest-job-ids-with-status-overview
source_filename: flink-rest-job-ids-with-status-overview-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-ids-with-status-overview-schema.json\",\n  \"title\": \"JobIdsWithStatusOverview\",\n  \"description\": \"JobIdsWithStatusOverview schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobIdWithStatus\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-ids-with-status-overview-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JobIdsWithStatusOverview
---
