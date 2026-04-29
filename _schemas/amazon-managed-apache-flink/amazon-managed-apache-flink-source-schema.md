---
description: For a SQL-based Kinesis Data Analytics application, describes the format of the data in the streaming source, and how each data element maps to corresponding columns created in the in-application stream.
layout: schema
name: SourceSchema
properties_list:
- description: ''
  name: RecordFormat
  type: object
- description: ''
  name: RecordEncoding
  type: object
- description: ''
  name: RecordColumns
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-source-schema-schema.json
slug: amazon-managed-apache-flink-source-schema
source_filename: amazon-managed-apache-flink-source-schema-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-source-schema-schema.json\",\n  \"title\": \"SourceSchema\",\n  \"description\": \"For a SQL-based Kinesis Data Analytics application, describes the format of the data in the streaming source, and how each data element maps to corresponding columns created in the in-application stream. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecordFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordFormat\"\n        },\n        {\n          \"description\": \"Specifies the format of the records on the streaming source.\"\n        }\n      ]\n    },\n    \"RecordEncoding\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordEncoding\"\n        },\n        {\n          \"description\": \"Specifies\
  \ the encoding of the records in the streaming source. For example, UTF-8.\"\n        }\n      ]\n    },\n    \"RecordColumns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordColumns\"\n        },\n        {\n          \"description\": \"A list of <code>RecordColumn</code> objects. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RecordFormat\",\n    \"RecordColumns\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-source-schema-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: SourceSchema
---
