---
description: Describes updates to the input streams, destination streams, and reference data sources for a SQL-based Kinesis Data Analytics application.
layout: schema
name: SqlApplicationConfigurationUpdate
properties_list:
- description: ''
  name: InputUpdates
  type: object
- description: ''
  name: OutputUpdates
  type: object
- description: ''
  name: ReferenceDataSourceUpdates
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-sql-application-configuration-update-schema.json
slug: amazon-managed-apache-flink-sql-application-configuration-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-sql-application-configuration-update-schema.json\",\n  \"title\": \"SqlApplicationConfigurationUpdate\",\n  \"description\": \"Describes updates to the input streams, destination streams, and reference data sources for a SQL-based Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputUpdates\"\n        },\n        {\n          \"description\": \"The array of <a>InputUpdate</a> objects describing the new input streams used by the application.\"\n        }\n      ]\n    },\n    \"OutputUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputUpdates\"\n        },\n        {\n          \"description\"\
  : \"The array of <a>OutputUpdate</a> objects describing the new destination streams used by the application.\"\n        }\n      ]\n    },\n    \"ReferenceDataSourceUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceDataSourceUpdates\"\n        },\n        {\n          \"description\": \"The array of <a>ReferenceDataSourceUpdate</a> objects describing the new reference data sources used by the application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-sql-application-configuration-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: SqlApplicationConfigurationUpdate
---
