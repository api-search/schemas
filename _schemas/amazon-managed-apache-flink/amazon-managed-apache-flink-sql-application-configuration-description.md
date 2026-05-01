---
description: Describes the inputs, outputs, and reference data sources for a SQL-based Kinesis Data Analytics application.
layout: schema
name: SqlApplicationConfigurationDescription
properties_list:
- description: ''
  name: InputDescriptions
  type: object
- description: ''
  name: OutputDescriptions
  type: object
- description: ''
  name: ReferenceDataSourceDescriptions
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-sql-application-configuration-description-schema.json
slug: amazon-managed-apache-flink-sql-application-configuration-description
source_filename: amazon-managed-apache-flink-sql-application-configuration-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-sql-application-configuration-description-schema.json\",\n  \"title\": \"SqlApplicationConfigurationDescription\",\n  \"description\": \"Describes the inputs, outputs, and reference data sources for a SQL-based Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDescriptions\"\n        },\n        {\n          \"description\": \"The array of <a>InputDescription</a> objects describing the input streams used by the application.\"\n        }\n      ]\n    },\n    \"OutputDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputDescriptions\"\n        },\n        {\n          \"description\"\
  : \"The array of <a>OutputDescription</a> objects describing the destination streams used by the application.\"\n        }\n      ]\n    },\n    \"ReferenceDataSourceDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceDataSourceDescriptions\"\n        },\n        {\n          \"description\": \"The array of <a>ReferenceDataSourceDescription</a> objects describing the reference data sources used by the application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-sql-application-configuration-description-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: SqlApplicationConfigurationDescription
---
