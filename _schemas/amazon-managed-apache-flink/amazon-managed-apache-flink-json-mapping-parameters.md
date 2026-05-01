---
description: For a SQL-based Kinesis Data Analytics application, provides additional mapping information when JSON is the record format on the streaming source.
layout: schema
name: JSONMappingParameters
properties_list:
- description: ''
  name: RecordRowPath
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-json-mapping-parameters-schema.json
slug: amazon-managed-apache-flink-json-mapping-parameters
source_filename: amazon-managed-apache-flink-json-mapping-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-json-mapping-parameters-schema.json\",\n  \"title\": \"JSONMappingParameters\",\n  \"description\": \"For a SQL-based Kinesis Data Analytics application, provides additional mapping information when JSON is the record format on the streaming source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecordRowPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordRowPath\"\n        },\n        {\n          \"description\": \"The path to the top-level parent that contains the records.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RecordRowPath\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-json-mapping-parameters-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: JSONMappingParameters
---
