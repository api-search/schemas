---
description: Describes updates for an SQL-based Kinesis Data Analytics application's input schema.
layout: schema
name: InputSchemaUpdate
properties_list:
- description: ''
  name: RecordFormatUpdate
  type: object
- description: ''
  name: RecordEncodingUpdate
  type: object
- description: ''
  name: RecordColumnUpdates
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-input-schema-update-schema.json
slug: amazon-managed-apache-flink-input-schema-update
source_filename: amazon-managed-apache-flink-input-schema-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-schema-update-schema.json\",\n  \"title\": \"InputSchemaUpdate\",\n  \"description\": \"Describes updates for an SQL-based Kinesis Data Analytics application's input schema.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecordFormatUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordFormat\"\n        },\n        {\n          \"description\": \"Specifies the format of the records on the streaming source.\"\n        }\n      ]\n    },\n    \"RecordEncodingUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordEncoding\"\n        },\n        {\n          \"description\": \"Specifies the encoding of the records in the streaming source; for example, UTF-8.\"\n        }\n   \
  \   ]\n    },\n    \"RecordColumnUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordColumns\"\n        },\n        {\n          \"description\": \"A list of <code>RecordColumn</code> objects. Each object describes the mapping of the streaming source element to the corresponding column in the in-application stream.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-schema-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: InputSchemaUpdate
---
