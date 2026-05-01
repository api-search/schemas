---
description: Describes the data format when records are written to the destination in a SQL-based Kinesis Data Analytics application.
layout: schema
name: DestinationSchema
properties_list:
- description: ''
  name: RecordFormatType
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-destination-schema-schema.json
slug: amazon-managed-apache-flink-destination-schema
source_filename: amazon-managed-apache-flink-destination-schema-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-destination-schema-schema.json\",\n  \"title\": \"DestinationSchema\",\n  \"description\": \"Describes the data format when records are written to the destination in a SQL-based Kinesis Data Analytics application. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecordFormatType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordFormatType\"\n        },\n        {\n          \"description\": \"Specifies the format of the records on the output stream.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RecordFormatType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-destination-schema-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: DestinationSchema
---
