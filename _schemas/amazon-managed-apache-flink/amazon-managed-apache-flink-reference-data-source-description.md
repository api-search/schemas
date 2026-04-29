---
description: For a SQL-based Kinesis Data Analytics application, describes the reference data source configured for an application.
layout: schema
name: ReferenceDataSourceDescription
properties_list:
- description: ''
  name: ReferenceId
  type: object
- description: ''
  name: TableName
  type: object
- description: ''
  name: S3ReferenceDataSourceDescription
  type: object
- description: ''
  name: ReferenceSchema
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-reference-data-source-description-schema.json
slug: amazon-managed-apache-flink-reference-data-source-description
source_filename: amazon-managed-apache-flink-reference-data-source-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-reference-data-source-description-schema.json\",\n  \"title\": \"ReferenceDataSourceDescription\",\n  \"description\": \"For a SQL-based Kinesis Data Analytics application, describes the reference data source configured for an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReferenceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The ID of the reference data source. This is the ID that Kinesis Data Analytics assigns when you add the reference data source to your application using the <a>CreateApplication</a> or <a>UpdateApplication</a> operation.\"\n        }\n      ]\n    },\n    \"TableName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/InAppTableName\"\n        },\n        {\n          \"description\": \"The in-application table name created by the specific reference data source configuration.\"\n        }\n      ]\n    },\n    \"S3ReferenceDataSourceDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ReferenceDataSourceDescription\"\n        },\n        {\n          \"description\": \"Provides the Amazon S3 bucket name, the object key name that contains the reference data. \"\n        }\n      ]\n    },\n    \"ReferenceSchema\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceSchema\"\n        },\n        {\n          \"description\": \"Describes the format of the data in the streaming source, and how each data element maps to corresponding columns created in the in-application stream.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ReferenceId\",\n    \"TableName\",\n    \"S3ReferenceDataSourceDescription\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-reference-data-source-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ReferenceDataSourceDescription
---
