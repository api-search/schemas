---
description: Describes the inputs, outputs, and reference data sources for a SQL-based Kinesis Data Analytics application.
layout: schema
name: SqlApplicationConfiguration
properties_list:
- description: ''
  name: Inputs
  type: object
- description: ''
  name: Outputs
  type: object
- description: ''
  name: ReferenceDataSources
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-sql-application-configuration-schema.json
slug: amazon-managed-apache-flink-sql-application-configuration
source_filename: amazon-managed-apache-flink-sql-application-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-sql-application-configuration-schema.json\",\n  \"title\": \"SqlApplicationConfiguration\",\n  \"description\": \"Describes the inputs, outputs, and reference data sources for a SQL-based Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Inputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Inputs\"\n        },\n        {\n          \"description\": \"The array of <a>Input</a> objects describing the input streams used by the application.\"\n        }\n      ]\n    },\n    \"Outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Outputs\"\n        },\n        {\n          \"description\": \"The array of <a>Output</a> objects describing the destination streams\
  \ used by the application.\"\n        }\n      ]\n    },\n    \"ReferenceDataSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceDataSources\"\n        },\n        {\n          \"description\": \"The array of <a>ReferenceDataSource</a> objects describing the reference data sources used by the application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-sql-application-configuration-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: SqlApplicationConfiguration
---
