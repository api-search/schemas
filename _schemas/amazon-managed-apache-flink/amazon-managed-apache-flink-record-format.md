---
description: For a SQL-based Kinesis Data Analytics application, describes the record format and relevant mapping information that should be applied to schematize the records on the stream.
layout: schema
name: RecordFormat
properties_list:
- description: ''
  name: RecordFormatType
  type: object
- description: ''
  name: MappingParameters
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-record-format-schema.json
slug: amazon-managed-apache-flink-record-format
source_filename: amazon-managed-apache-flink-record-format-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-record-format-schema.json\",\n  \"title\": \"RecordFormat\",\n  \"description\": \" For a SQL-based Kinesis Data Analytics application, describes the record format and relevant mapping information that should be applied to schematize the records on the stream. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecordFormatType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordFormatType\"\n        },\n        {\n          \"description\": \"The type of record format.\"\n        }\n      ]\n    },\n    \"MappingParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MappingParameters\"\n        },\n        {\n          \"description\": \"When you configure application input at the time of\
  \ creating or updating an application, provides additional mapping information specific to the record format (such as JSON, CSV, or record fields delimited by some delimiter) on the streaming source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RecordFormatType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-record-format-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: RecordFormat
---
