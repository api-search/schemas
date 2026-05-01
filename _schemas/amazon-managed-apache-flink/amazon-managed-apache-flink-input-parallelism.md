---
description: For a SQL-based Kinesis Data Analytics application, describes the number of in-application streams to create for a given streaming source.
layout: schema
name: InputParallelism
properties_list:
- description: ''
  name: Count
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-input-parallelism-schema.json
slug: amazon-managed-apache-flink-input-parallelism
source_filename: amazon-managed-apache-flink-input-parallelism-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-parallelism-schema.json\",\n  \"title\": \"InputParallelism\",\n  \"description\": \"For a SQL-based Kinesis Data Analytics application, describes the number of in-application streams to create for a given streaming source. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Count\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputParallelismCount\"\n        },\n        {\n          \"description\": \"The number of in-application streams to create.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-parallelism-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: InputParallelism
---
