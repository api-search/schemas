---
description: When you configure a SQL-based Kinesis Data Analytics application's input at the time of creating or updating an application, provides additional mapping information specific to the record format (such as JSON, CSV, or record fields delimited by some delimiter) on the streaming source.
layout: schema
name: MappingParameters
properties_list:
- description: ''
  name: JSONMappingParameters
  type: object
- description: ''
  name: CSVMappingParameters
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-mapping-parameters-schema.json
slug: amazon-managed-apache-flink-mapping-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-mapping-parameters-schema.json\",\n  \"title\": \"MappingParameters\",\n  \"description\": \"When you configure a SQL-based Kinesis Data Analytics application's input at the time of creating or updating an application, provides additional mapping information specific to the record format (such as JSON, CSV, or record fields delimited by some delimiter) on the streaming source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JSONMappingParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JSONMappingParameters\"\n        },\n        {\n          \"description\": \"Provides additional mapping information when JSON is the record format on the streaming source.\"\n        }\n      ]\n    },\n    \"CSVMappingParameters\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CSVMappingParameters\"\n        },\n        {\n          \"description\": \"Provides additional mapping information when the record format uses delimiters (for example, CSV).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-mapping-parameters-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: MappingParameters
---
