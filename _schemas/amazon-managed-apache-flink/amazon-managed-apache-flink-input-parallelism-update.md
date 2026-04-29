---
description: For a SQL-based Kinesis Data Analytics application, provides updates to the parallelism count.
layout: schema
name: InputParallelismUpdate
properties_list:
- description: ''
  name: CountUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-input-parallelism-update-schema.json
slug: amazon-managed-apache-flink-input-parallelism-update
source_filename: amazon-managed-apache-flink-input-parallelism-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-parallelism-update-schema.json\",\n  \"title\": \"InputParallelismUpdate\",\n  \"description\": \"For a SQL-based Kinesis Data Analytics application, provides updates to the parallelism count.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CountUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputParallelismCount\"\n        },\n        {\n          \"description\": \"The number of in-application streams to create for the specified streaming source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CountUpdate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-parallelism-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: InputParallelismUpdate
---
